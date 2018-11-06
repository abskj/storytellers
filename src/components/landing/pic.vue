<template>
    <div class="main yellow" v-bind:style="{ 'background-image': 'url(' + imurl + ')' }">
        <div class=inner debug></div>
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
  /* padding: 2%; */
  width:19%;
  margin:5px;
}

.inner{
  background-color: black;
}
.main:hover > .inner{
  transform: scale(1.1, 1.1);
  opacity: 50%;
}

.main{
  height:400px;
  overflow: hidden;
  background-size: cover;
  background-position: center;
}

img{
  vertical-align: middle;
  width: 99%;
  line-height: 100%;
}
</style>
