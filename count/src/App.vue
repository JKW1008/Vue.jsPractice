<script setup>
import { computed, ref } from "vue";
const cnt = ref(0);
const oddEven = computed(() => (cnt.value % 2 ? "Odd" : "Even"));
const counter = () => cnt.value++;
</script>
<template>
  <p>{{ cnt }}</p>
  <p>Odd or Even : {{ oddEven }}</p>
  <button @click="counter">click</button>
</template>
