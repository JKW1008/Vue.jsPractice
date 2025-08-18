<script setup>
import { ref } from "vue";

const titleClass = ref("");

const good = () => {
  titleClass.value = "title";
};

// function good() {
//   titleClass.value = "title";
// }
</script>
<template>
  <h1 :class="titleClass">Make me red</h1>
  <button @click="good">Click</button>
</template>
<style>
.title {
  color: red;
}
</style>
