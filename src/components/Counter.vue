<template>
  <div>Counter is: {{ counter }}</div>
  <button v-on:click="add">+</button>
  <button v-on:click="minus">-</button>
</template>
<script>
export default {
  data() {
    return {
      counter: 0,
    };
  },
  methods: {
    add() {
      this.counter++;
    },
    minus() {
      this.counter--;
    },
  },
};
</script>
<style lang=""></style>
