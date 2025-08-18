<script setup>
import { ref, computed } from "vue";
const cnt = ref(10);
const oddEven = computed(() => (cnt.value % 2 ? "Odd" : "Even"));
const counter = () => {
  cnt.value++;
};
</script>
<template>
  <p>cnt : {{ cnt }}</p>
  <p>odd or even : {{ oddEven }}</p>
  <button @click="counter">Click</button>
</template>
