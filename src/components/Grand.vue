<template>
  <input type="text" @keyup="$emit('my-keyup', $event, var1, var2)" />
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      var1: "var1",
      var2: "var2",
    };
  },
};
</script>
