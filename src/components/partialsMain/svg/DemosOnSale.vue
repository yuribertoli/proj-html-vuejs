<template>
  <div class="icons">

    <div class="block">
        <img src="../../../assets/img/iconaPhotoshoppata.png" alt="icona Demos">
        <span class="text">Demos</span>
    </div>

    <div class="block">
        <span class="number dollar">$</span>
        <span class="number">&nbsp;39</span>
        <span class="text">On Sale</span>
    </div>

  </div>
</template>

<script>
export default {
    name: "DemosOnSale"
}
</script>

<style scoped lang="scss">
.icons {
    position: absolute;
    right: 10px;
    top: 15%;

    .block {
        width: 40px;
        height: 40px;
        background-color: white;
        border-radius: 5px;
        margin-bottom: 5px;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        position: relative;
        &:hover {
            cursor: pointer;
        }

        img {
            width: 40%;
            height: auto;
            padding-bottom: 3px;
        }

        .number {
            color: #65bc7b;
            font-size: 1.1rem;
            font-weight: 700;
        }

        .number.dollar {
            font-size: 0.7rem;
            position: absolute;
            top: 4.5px;
            left: 7px;
        }

        .text {
            color: rgb(68, 68, 68);
            font-size: 0.5rem;
            font-weight: 600;
        }
    }
}

</style>