<template>
  <section class="cryptocard">
    <h2>VOOLA cryptocards</h2>

    <img class="cryptocard__image" src="../assets/images/group/Group.png" srcset="../assets/images/group/Group@2x.png" alt="group" />

    <div class="cryptocard__items">
      <article class="cryptocard__bag">
        <img class="cryptocard__img" src="../assets/images/bag/bag.png" srcset="../assets/images/bag/bag@2x.png" alt="bag" />
        <h3>
          Travel
          <p>Use of the VOOLA card without borders: automatic conversion of cryptocurrency and fiat. Payment for tickets and hotels through the</p>
        </h3>
      </article>

      <article class="cryptocard__filter">
        <img class="cryptocard__img" src="../assets/images/filter/filter.png" srcset="../assets/images/filter/filter@2x.png" alt="filter" />
        <h3>
          VOOLA technologes allow
          <p>Use of the VOOLA card is possible anywhere in the world where Mastercard, Visa, Union is supported pay.</p>
        </h3>
      </article>

      <article class="cryptocard__buy">
        <img class="cryptocard__img" src="../assets/images/buy/buy.png" srcset="../assets/images/buy/buy@2x.png" alt="buy" />
        <h3>
          Shopping
          <p>Use of the VOOLA card when making purchases</p>
        </h3>
      </article>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.cryptocard {
  align-items: center;
  color: var(--scheme-v2);
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin: calc(var(--scheme-gap) * 2) auto 0 auto;
  max-width: var(--scheme-max-width-wrapper);
  position: relative;

  h2 {
    text-align: center;
  }

  &__image {
    max-width: 492px;
    width: 100%;
    max-height: 596px;
    height: 100%;
  }

  &__img {
    width: 92px;
    height: 92px;
  }

  &__bag,
  &__buy,
  &__filter {
    display: flex;
    padding: 20px;
    position: absolute;
    margin: 0 40px;

    h3 {
      margin: 0 40px 0 0;
    }
    p {
      margin: 20px 0 0 0;
    }
  }

  &__bag,
  &__buy {
    h3 {
      margin: 0 0 0 40px;
    }
  }

  &__bag {
    width: 624px;
    top: 170px;
    right: -100px;
  }
  &__buy {
    width: 440px;
    top: 580px;
    right: 150px;
  }

  &__filter {
    text-align: right;
    width: 570px;
    top: 310px;
    left: -80px;

    img {
      order: 1;
    }
  }
}

@media only screen and(max-width:784px) {
  .cryptocard {
    &__items {
      display: flex;
      position: absolute;
      top: 370px;
      left: 0;
      margin: 20px;
    }
    &__filter {
      text-align: left;

      img {
        order: 0;
      }
    }
    &__bag,
    &__buy,
    &__filter {
      position: static;
      flex-direction: column;
      margin: 0 10px;
      background: rgba(255, 255, 255, 0.2);
      backdrop-filter: blur(6px);
      -webkit-backdrop-filter: blur(6px);
      border-radius: 28px;

      width: 244px;
      height: 224px;
      img {
        width: 60px;
        height: 60px;
      }

      h3 {
        font-size: 16px;
        margin: 20px 0 0 0;
      }
      p {
        font-size: 10px;
        margin: 10px 0 0 0;
      }
    }
  }
}
</style>
