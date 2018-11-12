<template>
  <div>
    <div class="whole">
      <div class="row r1">
        <nav>
        <div class="nav-wrapper">
          <ul id="nav-mobile" class="right hide-on-med-and-down">
            <li><a href="/stories">Stories</a></li>
            <li><a href="#">Storytellers</a></li>
            <li><a href="#">About Us</a></li>
          </ul>
        </div>
      </nav>
      </div>
      <div class="row main" >
        <div class="row brand center">
          STORYTELLERS
        </div>
        <div class="row message" >
          <div class="col s12 m4"></div>
          <div class="col s12 m4">
             <vue-typer
          :text='["create","show","relive","share"]'
          :repeat='Infinity'
          :shuffle='true'
          initial-action='erasing'
          :pre-type-delay='70'
          :type-delay='500'
          :pre-erase-delay='2000'
          :erase-delay='150'
          erase-style='backspace'
          :erase-on-complete='false'
          caret-animation='blink' 
      >
      </vue-typer>
      <mark>Original Art</mark>
    
          </div>
          <div class="col s12 m4">
            
          </div>
        </div>
      </div>
    </div>
    <div class="black">
      <gallery></gallery>
    </div>
    <app-footer></app-footer>
  </div>
</template>

<script>
import Gallery from "./landing/gallery.vue";
import Footer from "./landing/footer.vue";
import { VueTyper } from 'vue-typer'
export default {
  components: {
    gallery: Gallery,
    'app-footer' : Footer,
    'vue-typer': VueTyper
  }
};
</script>

<style>
    .whole {
      width: 100vw;
      height: 100vh;
      position: relative;
      top: 0px;
      background-image: linear-gradient(
          rgb(0, 0, 0,0.8),
          rgb(0, 0, 0,0.8)
        ),
        url("/static/images/hsda.jpg");
      background-size: cover;
      background-attachment: fixed;
    }
    .brand {
      margin-top: 25vh;
      font-family: "Megrim", cursive;
      font-size: 7em;
      color: rgb(255, 255, 255);
      font-weight: bolder;
    }
    .brand1 {
      position: absolute;
      font-size: 3em;
      top: 10px;
      font-family: "Megrim", cursive;
      color: rgb(255, 255, 255);
    }
    .message {
    
      font-family: "Megrim", cursive;
      font-size: 3.5em;
      color: rgb(255, 0, 0);
      border-radius: 10px;
      font-weight: bolder;
      /* box-shadow: 0px 0px 10px rgb(14, 13, 13); */
    }
    .vue-typer .custom.char {
  color: rgb(255, 255, 255);
  background-color: #1E1E1E;
}
    
    div:hover {
      border: 0px rgba(255, 0, 0, 0) solid;
    }
    nav {
      background-color: rgba(0, 0, 0, 0);
      padding-right: 50px;
    }
    nav * li a {
      font-family: "Megrim", cursive;
      font-size: 1.5em;
      margin-left: 1vw;
      margin-right: 1vw;
      margin-top: 2vh;
      border: 1px rgb(85, 0, 155) solid;
      border-radius: 5px;
      transition-duration: 100ms;
    }
    nav * li a:hover {
      box-shadow: 0px 0px 5px white;
      color: rgba(255, 255, 255, 0.685);
    }

    mark {
      font-weight: bolder;
    }
</style>
