<template>
    <div class="container">
        <div class="row">
            <h2 class="heading">
            {{title}}
        </h2>
        <h5 class="heading thin right" >
            {{creator}}
        </h5>
        </div>
        <div class="row">
            <div class="flow-text">
                {{content}}
            </div>
        </div>
    </div>
</template>

<script>
import Gallery from './../landing/gallery.vue'
export default {
    components:{
        'gallery' : Gallery
    },
    props:{
        content: {
            type: String
        },
        title:{

        },
        images: {
            type: Array
        },
        creator: {
            type: Array
        }
    }

}
</script>

<style>

</style>
