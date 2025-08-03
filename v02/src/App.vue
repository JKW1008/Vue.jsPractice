<script>
export default {
  data: function () {
    return {
      channel: "<b>왕초보 홈페이지 만들기</b>",
      subscribe: 2677,
    };
  },
};
</script>

<template>
  <h1 v-pre>채널명 : {{ channel }}</h1>
  <h2>구독자수 : {{ subscribe }}</h2>
  <p>오늘의 행운 숫자 : {{ Math.ceil(Math.random() * 45) }}</p>
  <p v-html="channel"></p>
  <h2 v-text="subscribe"></h2>
</template>

<style scoped></style>
