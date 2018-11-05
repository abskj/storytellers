<template>
    <div class="main yellow">
        <img :src="imurl">
    </div>
</template>

<script>
export default {
props:{
    imurl:{
        type:String
    }
},

mounted: function()
    {
        
    },
data(){
    return{

    }
}
}
</script>

<style scoped>
.main{
height: 200px;
width: 200px;
}
</style>
