<template>
  <h1>{{ str }}</h1>
  <h2>{{ arr[3] }} is number {{ arr[0] }}!</h2>
  <h3>{{ obj.val }} make building apps fun</h3>
</template>
<script>
export default {
  data() {
    return {
      str: "Hello World!", // str is being referenced in the h1 tag to display the value,
      arr: [1, 2, 3, "VueJs", "JavaScript"], //arr is being referenced in the h2 tag to display the value
      obj: { val: "Frameworks", val2: "programming" }, //obj is being referenced in the h3 tag to display the value
    };
  },
};
</script>
<style scoped></style>
