<template>
    <div>
        <pic v-bind:imurl="imurls[0]"></pic>
        
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
                'static/images/img1.jpg'
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
