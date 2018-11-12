<template>
    <div v-on:click="clickfunc" class="main yellow" v-bind:style="'background-image:url('+imurl+')'">
        <div class="inner"></div>
    </div>
</template>

<script>
export default {
  props: {
    imurl: {
      type: String
    },
    clickfunc:{
      type: Object
    },
  },

  mounted: function() {
    // alert(this.url);
  },
  data() {
    return {
      url:this.imurl,
    };
  }
};
</script>

<style scoped>
    .main{
      height:300px;
      overflow: hidden;
      background-size: cover;
      background-position: center;
    }

    .inner{
      background-color: black;
    }
    .main:hover{
      transform: scale(1.1, 1.1);
      opacity: 50%;
    }
</style>
