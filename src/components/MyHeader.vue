<template>
  <header>

    <div class="container">

        <div class="left-header">
            <img src="../assets/img/avadabarbers-logo-x2-300x104.png" alt="Logo Avada Barbers">
        </div>

        <div class="right-header">
            <nav>
                <ul>
                    <li v-for="(link, index) in navbar" :key="index">
                        <a :href="link.url">{{link.name}}</a>
                    </li>
                </ul>
            </nav>
        </div>
    
    </div>  

  </header>
</template>

<script>
export default {
    name: "MyHeader",

    props: {
        "navbar": Array
    },

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
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    z-index: 999;
    margin-top: 20px;
    
    .container {
        justify-content: space-between;

        .left-header {
            height: $height1;
            display: flex;
            align-items: center;

            img {
                width: 140px;
                height: auto;
                object-fit: contain;
            }
        }

        a {
            display: block;
            height: $height1;
            line-height: $height1;
            padding: 0 30px;
            margin: 0 10px;

            &:hover {
                box-shadow: 0 0 10px white;
                border-radius: 50%;
            }
        }
    }
}
</style>