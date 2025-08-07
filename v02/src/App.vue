<template>
  <div>
    <p>Full Name: {{ fullName }}</p>
    <input v-model="fullName" placeholder="Enter full name" />
    firstName : {{ firstName }} <br />
    lastNam : {{ lastName }}
  </div>
</template>

<script>
export default {
  data() {
    return {
      firstName: "John",
      lastName: "Doe",
    };
  },
  computed: {
    fullName: {
      get() {
        return this.firstName + " " + this.lastName;
      },
      set(newValue) {
        const names = newValue.split(" ");
        this.firstName = names[0];
        this.lastName = names[names.length - 1];
      },
    },
  },
};
</script>

<style></style>
