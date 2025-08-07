<script>
export default {
  data() {
    return {
      count: 0,
      y: "짝수",
    };
  },
  methods: {
    increment() {
      this.count++;
    },
  },
  watch: {
    count: {
      handler(newVal, oldVal) {
        console.log(`Count changed from ${oldVal} to ${newVal}`);
        if (newVal % 2 === 0) {
          this.y = "짝수";
        } else {
          this.y = "홀수";
        }
      },
      once: false,
    },
  },
};
</script>
<template>
  <p>Count : {{ count }}</p>
  <button @click="increment">Increment</button>
  <p>Result : {{ y }}</p>
</template>
<style></style>
