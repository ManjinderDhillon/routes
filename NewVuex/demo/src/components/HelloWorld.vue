<template>
  <h3>{{ $store.state.counter }}</h3>
  <button @click="addOne">Add</button>
</template>
<script>
export default {
  name: "HelloWorld",
  methods: {
    addOne() {
      this.$store.commit("increment");
      console.log(this.$store.state.counter);
    },
  },
};
</script>
