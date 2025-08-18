<script setup>
import { ref, watch } from "vue";
const obj = ref({ name: "홍길동", age: 30 });
const updateName = () => (obj.value.name = "Jason");
watch(
  obj,
  (newObj, oldObj) => {
    console.log(newObj, oldObj);
    // console.log("Chane the name, now name : " + newObj.name);
  },
  { immediate: true, deep: true }
);
</script>
<template>
  <h1>Profile</h1>
  <p>Name : {{ obj.name }}</p>
  <p>Age : {{ obj.age }}</p>
  <button @click="updateName">Change name</button>
</template>
