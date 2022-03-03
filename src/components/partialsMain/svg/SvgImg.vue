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

.svg-up-bw { /* per tutti i contenitori con la punta dell'img verso l'alto e come primo colore nero, poi bianco */
    .left {
      background-image: linear-gradient(to top left, white 50%, black 50%);
    }
    .right {
      background-image: linear-gradient(to top right, white 50%, black 50%);
    }
}

.svg-up-wb { /* per tutti i contenitori con la punta dell'img verso l'alto e come primo colore bianco, poi nero */
    .left {
      background-image: linear-gradient(to top left, black 50%, white 50%);
    }
    .right {
      background-image: linear-gradient(to top right, black 50%, white 50%);
    }
}

.svg-down-wg { /* per tutti i contenitori con la punta dell'img verso il basso e come primo colore bianco, poi grigio */
    .left {
      background-image: linear-gradient(to bottom left, white 50%, #f5f5f5 50%);
    }
    .right {
      background-image: linear-gradient(to bottom right, white 50%, #f5f5f5 50%);
    }
}

</style>