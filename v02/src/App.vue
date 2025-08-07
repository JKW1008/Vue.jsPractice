<script>
export default {
  data() {
    return {
      myWidth: 10,
    };
  },
  methods: {
    incWidth() {
      this.myWidth += 10;
    },
    initWidh() {
      this.myWidth = 10;
    },
  },
};
</script>

<template>
  <div
    class="demo"
    @mouseover="initWidh"
    :style="{ width: myWidth + 'px' }"
  ></div>
  <button @:click="incWidth">버튼을 클릭해 보세요.</button>
</template>

<style>
.demo {
  width: 100px;
  height: 100px;
  background-color: blueviolet;
}
</style>
