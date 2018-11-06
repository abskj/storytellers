<template>
  <div>
    <div class="whole">
      <div class="row r1">
        <nav>
        <div class="nav-wrapper">
          <ul id="nav-mobile" class="right hide-on-med-and-down">
            <li><a href="#">Stories</a></li>
            <li><a href="#">Storytellers</a></li>
            <li><a href="#">About Us</a></li>
          </ul>
        </div>
      </nav>
      </div>
      <div class="row main">
        <div class="row brand center">
          STORYTELLERS
        </div>
        <div class="row message center">
          <mark>
            Every artist tells a story through their art.
          But the artist also creates a story when they tell one.
          This is a place for those story tellers and some of us who want to be mesmerized by these stories.
          </mark>
        </div>
      </div>
    </div>
    <div style=" height:100vh;width:100vw;" class="black">
      <gallery></gallery>
    </div>
  </div>
</template>

<script>
import Gallery from "./landing/gallery.vue";
export default {
  components: {
    gallery: Gallery
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
      rgba(0, 0, 0, 0.952),
      rgba(71, 43, 6, 0.616)
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
  margin-left: 20vw;
  margin-right: 20vw;
  font-family: "Almendra Display", cursive;
  font-size: 2.5em;
  /* color: rgb(255, 230, 0); */
  border-radius: 10px;
  border: 0px rgb(146, 70, 8) solid;
  /* box-shadow: 0px 0px 10px rgb(14, 13, 13); */
}
.message mark {
  color: white;
  background-color: rgb(43, 13, 43);
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
</style>
