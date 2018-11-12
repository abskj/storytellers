<template>
    <div class="container" style="height:75vh">
        <div class="row">
            <h2 class="heading">
            {{title}}
        </h2>
        <h5 class="heading thin right" >
            {{creator}}
        </h5>
        </div>
        <div class="row">
            <div class="desc">
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
.desc{
    font-size: 1.4em;
    line-height: 1.6em;
}
</style>
