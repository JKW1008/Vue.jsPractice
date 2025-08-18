<script setup>
import { defineEmits } from "vue";

const emit = defineEmits(["customEvent"]);
const handleClick = () => {
  emit("customEvent", "Button clicked!");
};
</script>
<template>
  <button @click="handleClick">Click on me</button>
</template>
