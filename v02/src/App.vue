<script>
export default {
  data() {
    return {
      agree: false,
    };
  },
};
</script>

<template>
  <p>이 약관에 동의하십니까?</p>
  <input type="checkbox" v-model="agree" />
  {{ agree }}
  <button v-show="agree">가입하기</button>
</template>

<style></style>
