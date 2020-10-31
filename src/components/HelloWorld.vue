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
    onMykeyup(varr) {
      console.log(varr.event.target.value, " n ", varr.var1, " n ", varr.var2);
    },
  },
};
</script>
