<script setup>
import axios from "axios";
import { ref } from "vue";

const table = ref(null);

const inputData = () => {
  axios
    .post("http://localhost:3000/member", {
      name: "lee",
      email: "lee@gmail.com",
    })
    .then((res) => {
      console.log("complete");
    })
    .catch((err) => {
      console.log("server has error");
    });
  console.log("Hello");
};

const getData = () => {
  axios.get("http://localhost:3000/member").then((res) => {
    // console.log(res);
    const members = res.data;
    let htmlContent = `<table border = "1">
      <tr>
        <th>Id</th>
        <th>Name</th>
        <th>Email</th>
      </tr>`;
    members.forEach((member) => {
      htmlContent += `
      <tr>
        <td>${member.id}</td>
        <td>${member.name}</td>
        <td>${member.email}</td>
      </tr>
      `;
    });
    htmlContent += `</table>`;
    table.value.innerHTML = htmlContent;
  });
};
</script>
<template>
  <button @click="inputData">Input data</button>
  <button @click="getData">Get data</button>

  <div ref="table"></div>
</template>
<style scoped>
div {
  margin-top: 10px;
}
</style>
