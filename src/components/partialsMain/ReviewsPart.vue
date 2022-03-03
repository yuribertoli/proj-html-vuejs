<template>
  <div class="svg-down-wg">

    

    <div class="containerPartials">

        <h4>what people say</h4>
        <h2>reviews</h2>          
      
        <div class="display-containers">

        <div class="containerPartials services-items">

            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Aspernatur impedit optio vitae tempore, itaque dolorum. Ullam sunt blanditiis animi harum autem repellat qui eligendi, adipisci incidunt eos quibusdam? Aliquam, nemo.</p>

            <img src="../../assets/img/avadabarbers-trimcut-gallery6-400x400.jpg" alt="model">

            <span>John Doe</span>          

        </div>

        <div class="containerPartials services-items">

            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Aspernatur impedit optio vitae tempore, itaque dolorum. Ullam sunt blanditiis animi harum autem repellat qui eligendi, adipisci incidunt eos quibusdam? Aliquam, nemo.</p>

            <img src="../../assets/img/avadabarbers-trimcut-gallery7-400x402.jpg" alt="model">

            <span>Pete Jones</span>          

        </div>

        <div class="containerPartials services-items">

            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Aspernatur impedit optio vitae tempore, itaque dolorum. Ullam sunt blanditiis animi harum autem repellat qui eligendi, adipisci incidunt eos quibusdam? Aliquam, nemo.</p>

            <img src="../../assets/img/avadabarbers-trimcut-gallery3-400x402.jpg" alt="model">

            <span>Mark Wilson</span>      

        </div>

      </div>

    </div>

    <SvgImg/>

  </div>
</template>

<script>
import SvgImg from "./svg/SvgImg.vue"

export default {
    name: "ReviewsPart",

    components: {
      SvgImg
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/variables.scss";

.svg-down-wg {
    padding-top: 300px;

    .services-items {
        padding: 50px;
        width: $width3;

        img {
            height: 80px;
            width: auto;
            border-radius: 50%;
            margin: 10px 0;
        }

        span {
            color: $mainColor;
            font-style: italic;
            font-size: 0.7rem;
            font-weight: 600;
        }
    }
}

</style>