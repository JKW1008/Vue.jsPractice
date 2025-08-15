<script>
export default {
  data() {
    return {
      cnt: 0,
    };
  },
  computed: {
    oddEven() {
      return this.cnt % 2 ? "odd" : "even";
    },
  },
  methods: {
    counter() {
      this.cnt++;
    },
  },
};
</script>
<template>
  <p>{{ cnt }}</p>
  <p>Odd or Even : {{ oddEven }}</p>
  <button @click="counter">click</button>
</template>
