<template>

  <div class="svg-up-wb">

    <div class="containerPartials">

      <h4>mens grooming</h4>
      <h2>services</h2>

      <div class="display-containers">

        <div class="containerPartials services-items">

          <img src="../../assets/img/avadabarbers-trimcut-icon-before.png" alt="trimcut">

          <h3>trim &#38; cut</h3>

          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Aspernatur impedit optio vitae tempore, itaque dolorum. Ullam sunt blanditiis animi harum autem repellat qui eligendi, adipisci incidunt eos quibusdam? Aliquam, nemo.</p>

        </div>

        <div class="containerPartials services-items">

          <img src="../../assets/img/avadabarbers-washndry-icon.png" alt="barber soap">

          <h3>wash &#38; dry</h3>

          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Aspernatur impedit optio vitae tempore, itaque dolorum. Ullam sunt blanditiis animi harum autem repellat qui eligendi, adipisci incidunt eos quibusdam? Aliquam, nemo.</p>

        </div>

        <div class="containerPartials services-items">

          <img src="../../assets/img/avadabarbers-beardtrim-icon.png" alt="beard trimmer">

          <h3>beard tidy</h3>

          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Aspernatur impedit optio vitae tempore, itaque dolorum. Ullam sunt blanditiis animi harum autem repellat qui eligendi, adipisci incidunt eos quibusdam? Aliquam, nemo.</p>

        </div>

      </div>

      <button>read about our services</button>

    </div>

    <SvgImg/>

  </div>

</template>

<script>
import SvgImg from "./svg/SvgImg.vue"

export default {
    name: "ServicesPart",

    components: {
      SvgImg
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/variables.scss";

.container-partials {
  width: $width3;
}

.services-items {
  padding: 50px;

  img {
    height: 60px;
    width: auto;
  }
}


</style>