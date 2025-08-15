<script setup>
import { reactive, ref } from "vue";

const count = ref(0);

const obj1 = reactive({
  name: "kim",
  age: 33,
});

const good = () => {
  // count.value++;
  obj1.name = "lee";
};
</script>
<template>
  <p>count : {{ count }}</p>
  <p>obj1.name : {{ obj1.name }}</p>
  <p>obj1.age : {{ obj1.age }}</p>
  <button @click="good">click</button>
</template>
