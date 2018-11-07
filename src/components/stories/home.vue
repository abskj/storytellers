<template>
    <div>
        <div class="upper">
        <!-- Written summary of the art by the author -->
        <story :content="bigLorem" :title="lorem_title" :creator="lorem_artist"></story> 
    </div>
    <div class="lower">
        <!-- Navigational component that will take the user to  videos, pictures and everything else about the piece -->
    </div>
    </div>
</template>

<script>
import Story from './story.vue'

export default {
    components:{
        'story' : Story
    },
    computed:{
      bigLorem : function(){
            return (this.lorem+this.lorem+this.lorem+this.lorem+this.lorem+this.lorem+this.lorem)
      }  
    },
    data(){
        return {
            lorem : 'Lorem ipsum dolor sit amet vrhejvrehvjer vervre bvrbtbr sfdffe verggerg dgtbgtebg rvretcscfsfddffrg ghrrdwdwe nmnb  hbjh kbhjhbhjvrnkjbk kjbjrhevbje kbkhewb consectetur adipisicing elit. Labore cum, ut vel dolor unde non! Odit possimus eaque natus asperiores sapiente blanditiis repellat ad? Debitis quo ipsum dicta voluptas necessitatibus?',
            lorem_artist:'Abhishek Jha',
            lorem_title: 'A Beautiful Title',
        }
    }
}
</script>

<style scoped>
    .upper{
        max-height: 100px!important;
        width: 100vw;
    }
</style>
