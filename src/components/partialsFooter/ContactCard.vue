<template>
  <div class="containerPartials card">

    <img :src="require('../../assets/img/' + card.img)" :alt="card.alt">

    <button>{{card.text}}</button>

  </div>
</template>

<script>
export default {
    name: "ContactCard",

    props: {
        "card": Object
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/variables.scss";

.card {
    padding: 60px 0 ;

    img {
        width: 300px;
        height: auto;
    }

    button {
        margin: 30px 0;
    }
}
</style>