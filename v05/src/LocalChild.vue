<script>
export default {
  data() {
    return {
      c: 5,
    };
  },
  emits: ["createPost"],
};
</script>

<template>
  I'm Child component ( {{ c }} )
  <input type="text" ref="myInput" v-model="c" />
  <button @click="$emit('createPost', c)">Call parent's event</button>
</template>
