<script>
export default {
  data: function () {
    return {
      score: 55,
      subscribe: 2677,
    };
  },
};
</script>

<template>
  <!-- <h1 v-if="score >= 90">평점 : A</h1>
  <h1 v-else-if="score >= 80">평점 : B</h1>
  <h1 v-else-if="score >= 70">평점 : C</h1>
  <h1 v-else>평점 : F</h1> -->

  <h1 v-if="score != 60">이 영역은 v-if에서 처리하고 있습니다.</h1>
  <h1 v-show="score != 60">이 영역은 v-show에서 처리하고 있습니다.</h1>
</template>

<style></style>
