<template>
  <div class=green>
  <div class="main">asdfsadf{{ text }}</div></div>
</template>

<script>
export default {
  data() {
    return {
      text: "Copyright 2018"
    };
  },
  methods: {}
};
</script>

<style scoped>
div {
  height: 500px;
  width: 100%;
  border: 5px solid green;
}
</style>
