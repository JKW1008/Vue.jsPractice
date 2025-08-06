<script>
export default {
  data() {
    return {
      sports: ["Baseball", "Football", "Volleyball", "Swimming"],
    };
  },
};
</script>

<template>
  <ul>
    <li v-for="sport in sports">{{ sport }}</li>
  </ul>
</template>

<style></style>
