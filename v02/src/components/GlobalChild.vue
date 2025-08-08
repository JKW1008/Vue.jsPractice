<script>
export default {
  beforeCreate() {
    console.log("GlobalComponent beforeCreate");
  },
  created() {
    console.log("GlobalComponent created");
  },
  beforeMount() {
    console.log("GlobalComponent beforeMount");
  },
  mounted() {
    console.log("GlobalComponent mounted");
  },
  updated() {
    console.log("GlobalComponent updated");
  },
  beforeUnmount() {
    console.log("GlobalComponent beforeUnmount");
  },
  unmounted() {
    console.log("GlobalComponent unmounted");
  },
};
</script>

<template>
  <h1>Global Component</h1>
  <p>it's Global Component</p>
</template>
<style scoped>
h1 {
  color: red;
}

p {
  color: orange;
}
</style>
