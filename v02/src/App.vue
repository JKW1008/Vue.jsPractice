<script>
import LocalComponent from "./components/LocalChild.vue";
export default {
  components: {
    LocalComponent,
  },
};
</script>
<template>
  <h1>App.Vue</h1>
  <LocalComponent />
  <GlobalChild />
</template>
<style></style>
