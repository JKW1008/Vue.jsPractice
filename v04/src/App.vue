<script>
import ChildCom from "./ChildComponent.vue";
export default {
  data() {
    return {
      name: "John",
      age: 30,
    };
  },
  components: {
    ChildCom,
  },
  methods: {
    ageInc() {
      this.age++;
    },
  },
};
</script>
<template>
  <h1>I'm parents</h1>
  <button @click="ageInc">age ++</button>
  <ChildCom v-bind:name="name" v-bind:age="age" />
</template>
<style></style>
