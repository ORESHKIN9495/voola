<template>
  <section class="service">
    <h2>What does <b>VOOLA</b> give you?</h2>
    <picture class="service__logo">
      <img src="../assets/images/logotype/logotype.png" srcset="../assets/images/logotype/logotype@2x.png" alt="logo" />
    </picture>

    <card />
  </section>
</template>

<script>
import Card from './card.vue'
export default {}
</script>

<style lang="scss" scoped>
.service {
  color: var(--scheme-v2);
  margin: var(--scheme-gap) auto;
  max-width: var(--scheme-max-width-wrapper);
  position: relative;
  padding: 20px;

  &__logo {
    display: flex;
    z-index: -1;
    position: absolute;
    top: -40px;
    right: -120px;

    img {
      height: 304px;
    }
  }
}
</style>
