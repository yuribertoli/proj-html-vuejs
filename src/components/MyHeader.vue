<template>
  <header>

    <div class="container">

        <div class="left-header">
            <img src="../assets/img/avadabarbers-logo-x2-300x104.png" alt="Logo Avada Barbers">
        </div>

        <div class="right-header">

        </div>
    
    </div>  

  </header>
</template>

<script>
export default {
    name: "MyHeader",

    data(){
        return{

        }
    },

    methods: {

    }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";

header {
    height: $height1;
    background-color: red;
    
    .container {
        justify-content: space-between;

        .left-header {
            height: $height1;
            display: flex;
            align-items: center;

            img {
                width: 200px;
                height: auto;
                object-fit: contain;
            }
        }

        .right-header {
            
        }
    }
}
</style>