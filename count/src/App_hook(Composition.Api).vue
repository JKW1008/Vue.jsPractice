<script>
import { computed, ref } from "vue";
export default {
  setup() {
    const cnt = ref(0);
    const oddEven = computed(() => (cnt.value % 2 ? "Odd" : "Even"));
    const counter = () => cnt.value++;

    return {
      cnt,
      oddEven,
      counter,
    };
  },
};
</script>
<template>
  <p>{{ cnt }}</p>
  <p>Odd or Even : {{ oddEven }}</p>
  <button @click="counter">click</button>
</template>
