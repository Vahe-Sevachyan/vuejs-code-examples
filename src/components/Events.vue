<template>
  <div>
    <input
      v-on:input="setValue"
      type="text"
      placeholder="enter number to double"
    />
    <br />
    <button v-on:click="add()">Add</button>
    <button v-on:click="subtract()">Subtract</button>
    <button v-on:click="double()">Double</button><br />

    <p>The Count Doubled: {{ counter }}</p>

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

    setValue(event) {
      this.doubleVal = event.target.value;
    },
    double() {
      if (this.counter === 0) {
        this.counter = this.doubleVal * 2;
      } else {
        this.counter = this.counter * 2;
      }
    },
  },
};
</script>
<style scoped>
button {
}
</style>
