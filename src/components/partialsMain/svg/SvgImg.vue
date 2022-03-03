<template>
  <div class="svg">
    <div class="left"></div>
    <div class="right"></div>
  </div>
</template>

<script>
export default {
    name: "SvgImg"
}
</script>

<style scoped lang="scss">
@import "../../../assets/style/variables.scss";

/* Regole generali dimensioni e posizionamento */
.svg {
    display: flex;

    .left, .right {
      width: $width2;
      height: $height1;
    }
}

/* Regole colori e direzione in base a dove posizionate */
.pro-barbers {
    .left {
      background-image: linear-gradient(to top left, white 50%, black 50%);
    }
    .right {
      background-image: linear-gradient(to top right, white 50%, black 50%);
    }
}


</style>