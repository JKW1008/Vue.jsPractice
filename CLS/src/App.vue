<script setup>
import ChildComponent from "@/components/ChildComponent.vue";

const handleCustomEvent = (message) => {
  console.log("Received event: " + message);
};
</script>
<template><ChildComponent @custom-event="handleCustomEvent" /></template>
