<script>
export default {
  data() {
    return {
      inputName: "홍길동",
    };
  },
};
</script>

<template>
  <input type="text" v-model="inputName" />
  <p>{{ inputName }}</p>
</template>

<style></style>
