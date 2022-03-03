<template>
  <div class="jumbotron">
    <div class="container">

      <div class="left-jumbotron">
        <h1>Barber Shop</h1>
        <hr>
        <span>The Pinnacle of Male Grooming</span>
        <button>Learn More</button>
      </div>

      <div class="right-jumbotron">
        <img src="../../assets/img/avadabarbers_hero_focalmirror-800x1100.png" alt="barber at work">
      </div>

    </div>
  </div>
</template>

<script>
export default {
    name: "MyJumbotron",

    data(){
        return{

        }
    },

    methods: {
        
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/variables.scss";

.jumbotron {
  height: $jumbotronHeight;
  background-image: url("../../assets/img/avadabarbers-homepage-hero-bg.jpg");
  background-size: cover;
  position: relative;
  z-index: -3;

  .container {
    height: calc($jumbotronHeight);
    padding-top: $height2;

    .left-jumbotron, .right-jumbotron {
      width: $width2;
    }

    .left-jumbotron {
      display: flex;
      flex-direction: column;
      justify-content: center;

      h1 {
        color: white;
        font-size: 4rem;
        font-family: 'Playfair Display', serif;
      }

      hr {
        color: $mainColor;
        height: 2px;
        background-color: $mainColor;
        width: calc($width3 + 30px);
        margin: 20px 0;
      }

      span {
        color: #505050;
        margin-bottom: 20px;
      }
    }

    .right-jumbotron {
      display: flex;

      img {
        width: 70%;
        height: auto;
        margin: auto;
      }
    }
  }
}
</style>