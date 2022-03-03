<template>
  <div class="copyright">
      <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere hic error eum laudantium rerum mollitia.</span>
  </div>
</template>

<script>
export default {
    name: "CopyRight"
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/variables.scss";

.copyright {
    height: $height1;
    text-align: center;
    
    span {
        color: gray;
        line-height: $height1;
        font-size: 0.6rem;
        color: rgb(60, 60, 60);
    }
}
</style>