<script setup>
import ButtonCounter from "@/components/ButtonCounter.vue";

const post = {
  id: 1,
  title: "This is title",
  mainCont: "This is main content",
};
</script>
<template>
  <h1>The components below are child components.</h1>
  <ButtonCounter :title="post.title" :mainCont="post.mainCont" />
</template>
