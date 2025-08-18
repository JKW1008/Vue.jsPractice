<script setup>
import axios from "axios";

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
</script>
<template>
  <button @click="inputData">Input data</button>
</template>
