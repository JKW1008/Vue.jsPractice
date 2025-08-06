<script>
export default {
  data() {
    return {
      click_yes: true,
    };
  },
  methods: {
    createAlert() {
      if (this.click_yes) {
        alert("경고창이 떴습니다.");
      }
    },
  },
};
</script>

<template>
  <button v-on:click.once="createAlert">Click</button>
</template>

<style></style>
