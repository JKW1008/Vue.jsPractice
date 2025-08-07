<script>
export default {
  data() {
    return {
      chk: false,
    };
  },
  computed: {
    yesNo() {
      if (this.chk) {
        return "yes";
      } else {
        return "no";
      }
    },
  },
};
</script>

<template>
  <input type="checkbox" v-model="chk" /> {{ yesNo }} {{ yesNo }} {{ yesNo }}
</template>

<style></style>
