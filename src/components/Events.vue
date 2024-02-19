<template>
  <div>
    <button v-on:click="add()">Add</button>
    <button v-on:click="subtract()">Subtract</button>
    <button v-on:click="double()">Double</button>
    <input v-on:input="setName" type="text" />
    <p>Count is: {{ counter }}</p>
  </div>
</template>
<script>
export default {
  data() {
    return {
      counter: 0,
      doubleVal: 0,
    };
  },
  methods: {
    add() {
      return this.counter++;
    },
    subtract() {
      return this.counter--;
    },

    setName(event) {
      this.doubleVal = event.target.value;
    },
    double() {
      this.counter = this.doubleVal * 2;
    },
  },
};
</script>
<style scoped></style>
