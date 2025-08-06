<script>
export default {
  data() {
    return {
      kValue: "",
    };
  },
  methods: {
    getKey(e) {
      this.kValue = e.key;
      alert("control + s 를 누르셨습니다.");
    },
  },
};
</script>

<template>
  <input type="text" v-on:keydown.control.s="getKey" /><br />
  <span>{{ kValue }}</span>
</template>

<style></style>
