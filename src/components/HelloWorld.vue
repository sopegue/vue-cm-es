<template>
  <Grand @my-keyup.enter="onMykeyup"></Grand>
</template>

<script>
import Grand from "@/components/Grand.vue";

export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
  components: {
    Grand,
  },
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    onMykeyup(e, var1, var2) {
      console.log(e.target.value, " n ", var1, " n ", var2);
    },
  },
};
</script>
