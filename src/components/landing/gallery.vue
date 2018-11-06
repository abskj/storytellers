<template>
    <div>
        <div v-for="im in imurls">
            <pic v-bind:imurl="im"></pic>
            
        </div>
    </div>
</template>

<script>
import Pic from './pic.vue'
export default {
components:{
'pic' :Pic
},
 data(){
        return {
            imurls : [
                'https://cdn.acidcow.com/pics/20131213/weird_and_awkward_stock_photos_06.jpg',
                'https://cdn.acidcow.com/pics/20131213/weird_and_awkward_stock_photos_13.jpg'
            ]
        }
    },
methods:{
   
}
}
</script>

<style scoped>
.main{

}
</style>
