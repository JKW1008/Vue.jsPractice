<script>
export default {
  props: ["name", "age"],
  created() {
    console.log(this.name);
    console.log(this.age);
  },
  methods: {
    propsUpdater() {
      this.age = 30;
    },
  },
};
</script>
<template>
  <h1>Child component</h1>
  <p>Name : {{ name }}</p>
  <p>Age : {{ age }}</p>
</template>
