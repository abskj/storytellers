<template>
    <div class="main yellow">
        <img :src="imurl">
    </div>
</template>

<script>
export default {
  props: {
    imurl: {
      type: String
    }
  },

  mounted: function() {},
  data() {
    return {};
  }
};
</script>

<style scoped>
.main {
  float: left;
  padding: 2%;
}

.main img:hover {
  transform: scale(1.1, 1.1);
}
</style>
