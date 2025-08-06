<script>
export default {
  data: function () {
    return {
      userName: "왕초보",
    };
  },
  methods: {
    greeting(userName) {
      return " Hi, there " + userName;
    },
  },
};
</script>

<template>
  <h1>{{ greeting("Tom") }}</h1>
</template>

<style></style>
