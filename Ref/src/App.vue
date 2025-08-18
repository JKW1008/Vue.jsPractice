<script setup>
import { ref } from "vue";

const a = ref(null);
const good = () => {
  alert(a.value.innerText);
  alert(document.getElementById("b").innerText);
};
</script>
<template>
  <h1 ref="a" id="b">Hi, I'm KingChobo make home page</h1>
  <button @click="good">click</button>
</template>
