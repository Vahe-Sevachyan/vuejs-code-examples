<template>
  <div>
    <button v-on:click="add()">Add</button>
    <button v-on:click="subtract()">Subtract</button>
    <button v-on:click="double()">Double</button><br />
    <input
      v-on:input="setName"
      type="text"
      placeholder="enter number to double"
    />
    <p>Count is: {{ counter }}</p>

    <input v-on:input="setName" type="text" placeholder="Enter name..." />
    <p>Name is: {{ name }}</p>
  </div>
</template>
<script>
export default {
  data() {
    return {
      counter: 0,
      doubleVal: 0,
      name: "",
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
    setName(event) {
      this.name = event.target.value;
    },
  },
};
</script>
<style scoped>
button {
}
</style>
