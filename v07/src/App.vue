<script>
import FancyButton from "@/components/FancyButton.vue";
import MainLayout from "@/MainLayout.vue";

export default {
  components: {
    FancyButton,
    MainLayout,
  },
};
</script>
<template>
  <h1>I'm App.vue</h1>
  <MainLayout>
    <template #header>
      <h1>Header</h1>
    </template>
    <template #contents>
      <h1>Contents</h1>
    </template>
    <template #footer>
      <h1>Footer</h1>
    </template>
  </MainLayout>
  <FancyButton><strong>click3</strong></FancyButton>
</template>
<style></style>
