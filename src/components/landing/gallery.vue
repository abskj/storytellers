<template>
    <div debug>
        <div v-for="im in imurls" :key="im.key">
            <pic v-bind:imurl="im.text" :key="im.key"></pic>
            
        </div>
    </div>
</template>

<script>
import Pic from "./pic.vue";
export default {
  components: {
    pic: Pic
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
        }
      ]
    };
  },
  methods: {}
};
</script>

<style scoped>

</style>
