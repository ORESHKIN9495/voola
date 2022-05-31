<template>
  <section class="service">
    <div class="service__wrapper">
      <h2>What does <span>VOOLA</span> give you?</h2>

      <div class="service__img">
        <img src="../assets/images/logotype/logotype.png" srcset="../assets/images/logotype/logotype@2x.png" alt="logo" />
      </div>

      <card />
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.service {
  &__wrapper {
    margin: var(--scheme-gap) auto;
    max-width: var(--scheme-max-width-wrapper);
    padding: 20px;

    h2 {
      margin: 0 0 40px 0;
    }
    span {
      font-weight: bold;
    }
  }
  &__img {
    left: 50%;
    position: absolute;
    transform-origin: 0 0;
    top: -30px;
    vertical-align: top;
    width: 100%;

    img {
      height: 304px;
    }
  }
}

@media only screen and(max-width:740px) {
  .service {
    h2 {
      font-size: 36px;
      text-align: center;
    }

    &__img {
      top: 1220px;
      transform: rotate(-90deg) translateY(-50%);

      img {
        height: 325px;
        width: 880px;
      }
    }
  }
}
</style>
