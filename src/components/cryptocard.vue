<template>
  <section class="cryptocard">
    <h2>VOOLA cryptocards</h2>

    <img class="cryptocard__image" src="../assets/images/group/Group.png" srcset="../assets/images/group/Group@2x.png" alt="group" />

    <cardslider class="cryptocard__slider" />
  </section>
</template>

<script>
import cardslider from './cardslider.vue'
export default {
  components: { cardslider },
}
</script>

<style lang="scss" scoped>
.cryptocard {
  align-items: center;
  color: var(--scheme-v2);
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin: calc(var(--scheme-gap) * 2) auto;
  max-width: var(--scheme-max-width-wrapper);
  position: relative;

  h2 {
    text-align: center;
  }

  &__image {
    max-width: 492px;
    width: 100%;
  }

  &__slider {
    position: absolute;
    bottom: 0;
    right: 0;
    top: 0;
    left: 0;
  }
}

@media only screen and(max-width:740px) {
  .cryptocard {
    h2 {
      font-size: 28px;
    }
    &__slider {
      position: absolute;
      bottom: inherit;
      top: 70%;
    }
  }
}
</style>
