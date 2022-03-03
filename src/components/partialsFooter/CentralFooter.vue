<template>
  <div class="containerPartials central-footer">

    <img src="../../assets/img/avadabarbers-logo-x2-300x104.png" alt="Logo Avada Barbers">

    <ul class="containerPartials">
        <li v-for="(item, index) in info" :key="index"> <!-- metto in colonna le info dell'azienda -->
            {{item.text}}   
        </li>
    </ul>

    <h4>follow us</h4>

    <div class="social">
        <ul>
            <li v-for="(social, index) in socials" :key="index">
                <i :class="social.class"></i> <!-- popolo dinamicamente la classe del tag "i" per creare le icone di FontAwesome -->
            </li>
        </ul>
    </div>

  </div>
</template>

<script>
export default {
    name: "CentralFooter",

    props: {
        "info": Array,
        "socials": Array
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/variables.scss";

.central-footer {

    img {
        width: 140px;
        height: auto;
        object-fit: contain;
    }

    ul.containerPartials {
        padding: 50px 0 40px;

        li {
            color: rgb(87, 85, 85);
            font-size: 0.7rem;
            line-height: 16px;
        }
    }

    .social ul {
        display: flex;
        margin-top: 40px;

        li {
            color: #bebdbd;
            margin: 0 10px;

            &:hover {
                color: white;
                cursor: pointer;
            }
        }
    }
}
</style>