<template>

    <div class="groom">

        <div class="containerPartials">

            <h4>we have you covered</h4>
            <h2>avada grooming products</h2>

            <div class="display-containers">

            <div class="containerPartials services-items">

                <img src="../../assets/img/brush_dark-800x800.png" alt="brush">

                <h3>brush</h3>

                <span>$15.00</span>

            </div>

            <div class="containerPartials services-items">

                <img src="../../assets/img/scissors-800x800.png" alt="scissors">

                <h3>scissors</h3>

                <span>$15.00</span>

            </div>

            <div class="containerPartials services-items">

                <img src="../../assets/img/hot_oil_dark-800x800.png" alt="hot oil">

                <h3>hot oil</h3>

                <span>$85.00</span>

            </div>

            <div class="containerPartials services-items">

                <img src="../../assets/img/straight_razor_dark-800x800.png" alt="straight razor">

                <h3>straight razor</h3>

                <span>$30.00</span>

            </div>

            </div>

            <button>shop our product range</button>

        </div>
    </div>    
</template>

<script>
export default {
    name: "GroomingProducts"
}
</script>

<style scoped lang="scss">
@import "../../assets/style/variables.scss";

.groom {
    background-image: url("../../assets/img/avadabarbers-reviewsbackground.jpg");
    background-size: cover;

    .services-items {
        padding: 50px 10px;
        width: $width4;

        img {
            height: 250px;
            width: auto;
        }

        span {
            color: $mainColor;
            font-weight: 100;
            font-size: 0.8rem;
        }
    }
}
</style>