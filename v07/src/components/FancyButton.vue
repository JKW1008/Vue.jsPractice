<script>
export default {
  //   props: ["buttonname"],
  data() {
    return {
      buttonname: "goodbye!!!",
    };
  },
};
</script>
<template>
  <button class="fancy-btn">
    <slot :buttonname>default string</slot>
  </button>
</template>
