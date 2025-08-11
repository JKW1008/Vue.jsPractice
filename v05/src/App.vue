<script>
import LocalChild from "@/LocalChild.vue";
export default {
  data() {
    return {
      c: 0,
    };
  },
  components: {
    LocalChild,
  },
  methods: {
    callFunction(var1) {
      console.log("Event called from child component");
      console.log("child component : " + var1);
      this.c = var1;
    },
  },
};
</script>
<template>
  <h1>I'm parent compontent. ( {{ c }} )</h1>
  <LocalChild @create-post="callFunction" />
</template>
<style></style>
