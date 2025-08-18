<script setup>
import { ref, watchEffect } from "vue";

const count = ref(1);
const name = ref("Jason");
const counter = () => count.value++;
const updateName = () =>
  (name.value = name.value == "Jason" ? "Mike" : "Jason");

watchEffect(() => {
  console.log(`Count is ${count.value}. The name was ${name.value}`);
});
</script>
<template>
  <p>watchEffect</p>
  <p>count : {{ count }}</p>
  <p>name : {{ name }}</p>
  <button @click="counter">Click</button>
  <button @click="updateName">Change Name</button>
</template>
