<template>
  <div>
    <button v-on:click="add()">Add</button>
    <button v-on:click="subtract()">Subtract</button>
    <p>Count is: {{ counter }}</p>
  </div>
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
      return this.counter++;
    },
    subtract() {
      return this.counter--;
    },
  },
};
</script>
<style scoped></style>
