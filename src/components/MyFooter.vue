<template>
  <footer>

    <div class="container">

      <ContactCard :card="cards.shop"/> <!-- smisto gli oggetti che mi servono per ogni card -->
      <CentralFooter :info="info" :socials="socials"/> 
      <ContactCard :card="cards.book"/> <!-- smisto gli oggetti che mi servono per ogni card -->

    </div>

    <div class="bottom-footer">

      <CopyRight/>

    </div>

  </footer>
</template>

<script>
import ContactCard from "./partialsFooter/ContactCard.vue";
import CentralFooter from "./partialsFooter/CentralFooter.vue";
import CopyRight from "./partialsFooter/CopyRight.vue";

export default {
    name: "MyFooter",

    props: {
      "cards": Object,
      "info": Array,
      "socials": Array
    },

    components: {
      ContactCard,
      CentralFooter,
      CopyRight
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";

footer {
  background-color: #121314;

  .container * {
    width: $width3;
  }

  .bottom-footer {
    background-color: #161718;
    height: $height1;
  }
}

</style>