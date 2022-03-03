<template>
  <div class="contain">

    <div class="left">
        <div class="overlay"></div>
        <img src="../../assets/img/shaving_butter-800x800.png" alt="shaving butter">
    </div>

    <div class="right">

        <div class="containerPartials shave-butter">

            <h4>this month featured product</h4>
            <h2>shaving butter</h2>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti quam eos odit recusandae ab sit molestiae doloribus. Consequuntur, necessitatibus atque.</p>
            <button>buy now</button>

        </div>

    </div>

  </div>
</template>

<script>
export default {
    name: "ShavingButter"
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/variables.scss";
$leftWidth: 40%;

.contain {
    display: flex;
    height: 300px;

    .left, .right {
        height: 100%;
    }

    .left {
        width: $leftWidth;
        background-image: url("../../assets/img/avadabarbers-second-blog-700x441.jpg");
        background-size: cover;
        background-position-x: center;
        position: relative;
        filter: grayscale(100%);

        .overlay {
            position: absolute;
            top: 0;
            left: 0;
            bottom: 0;
            right: 0;
            background-color: rgba(0, 0, 0, 0.5);
        }

        img {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 90%;
            z-index: 3;
        }
    }

    .right {
        width: calc(100% - $leftWidth);
        background-color: black;

        .shave-butter {
            padding: 40px 0;
            align-items: flex-start;

            h4 {
                margin-top: 10px;
            }

            h2 {
                padding-top: 0;
            }

            p {
                text-align: start;
                margin-bottom: 10px;
            }
        }
    }
}

</style>