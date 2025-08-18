<script setup>
import { onMounted, ref } from "vue";

// const props = defineProps(["title", "mainCont"]);
// const props = defineProps({
//   title: String,
//   mainCont: String,
// });
const props = defineProps({
  title: {
    type: String,
    required: true,
  },
  mainCont: {
    type: String,
    required: true,
  },
});

const title = ref("");
const cont = ref("");

onMounted(() => {
  title.value = props.title;
  cont.value = props.mainCont;
});
</script>
<template>
  <p>Title : {{ title }}</p>
  <p>Cont : {{ cont }}</p>
</template>
