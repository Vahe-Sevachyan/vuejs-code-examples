<template>
  <h1>{{ str }}</h1>
  <h2>{{ arr[3] }} is number {{ arr[0] }}!</h2>
  <h3>{{ obj.val }} make building apps fun</h3>
  <p>Here i am linking to <a v-bind:href="url">url</a></p>
</template>
<script>
export default {
  data() {
    return {
      str: "Hello World!", // str is being referenced in the h1 tag using the double curly braces to display the value,
      arr: [1, 2, 3, "VueJs", "JavaScript"], //arr is being referenced in the h2 tag using the double curly braces to display the value
      obj: { val: "Frameworks", val2: "programming" }, //obj is being referenced in the h3 tag using the double curly braces to display the value
      url: "https://www.google.com", //url is being referenced in the anchor tag and is bound to the href attribute using v-bind
    };
  },
};
</script>
<style scoped></style>

//interpolation is how you output data stored in a value which can be a string,
array, object or boolean.
