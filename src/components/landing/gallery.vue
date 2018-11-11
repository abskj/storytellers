<template>
    <div :class="wrap">
        <div v-for="im in imurls" :key="im.key" style="word-wrap:break-word">
            <pic v-bind:imurl="im.text" :key="im.key" v-bind:clickfunc="clickfunc"></pic>
        </div>
    </div>
</template>

<script>
import Pic from "./pic.vue";
export default {
  components: {
    pic: Pic
  },
  methods:{
    clickfunc:function() {
      alert("Ok");
    },
  },
  computed:{
    wrap: function(){
      return 'wrap'
    }
  },
  data() {
    return {
      imurls: [
        {
          key: 0,
          text:
            "https://cdn.acidcow.com/pics/20131213/weird_and_awkward_stock_photos_06.jpg"
        },
        {
          key: 1,
          text:
            "https://cdn.acidcow.com/pics/20131213/weird_and_awkward_stock_photos_13.jpg"
        },
        {
          key: 0,
          text:
            "https://cdn.acidcow.com/pics/20131213/weird_and_awkward_stock_photos_06.jpg"
        },
        {
          key: 1,
          text:
            "https://cdn.acidcow.com/pics/20131213/weird_and_awkward_stock_photos_13.jpg"
        },
        {
          key: 0,
          text:
            "https://cdn.acidcow.com/pics/20131213/weird_and_awkward_stock_photos_06.jpg"
        },
        {
          key: 1,
          text:
            "https://cdn.acidcow.com/pics/20131213/weird_and_awkward_stock_photos_13.jpg"
        },
        {
          key: 0,
          text:
            "https://cdn.acidcow.com/pics/20131213/weird_and_awkward_stock_photos_06.jpg"
        },
        {
          key: 1,
          text:
            "https://cdn.acidcow.com/pics/20131213/weird_and_awkward_stock_photos_13.jpg"
        },
        {
          key: 0,
          text:
            "https://cdn.acidcow.com/pics/20131213/weird_and_awkward_stock_photos_06.jpg"
        },
        {
          key: 1,
          text:
            "https://cdn.acidcow.com/pics/20131213/weird_and_awkward_stock_photos_13.jpg"
        },
        {
          key: 0,
          text:
            "https://cdn.acidcow.com/pics/20131213/weird_and_awkward_stock_photos_06.jpg"
        },
        {
          key: 1,
          text:
            "https://cdn.acidcow.com/pics/20131213/weird_and_awkward_stock_photos_13.jpg"
        }
      ]
    };
  },
};
</script>

<style scoped>
 .wrap{
      display: grid;
      grid-column-gap: 20px;
      grid-row-gap: 20px;
      grid-template-columns: repeat(auto-fit, 300px);
      justify-content: center;
      align-items:center;
      padding: 20px 20px;
    }  
</style>
