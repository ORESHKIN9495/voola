<template>
  <section class="cardslider" :style="{ marginLeft: `${index}px` }">
    <article class="cardslider__bag" @click="next">
      <img class="cardslider__img" src="../assets/images/bag/bag.png" srcset="../assets/images/bag/bag@2x.png" alt="bag" />

      <h3>
        Travel
        <p>Use of the VOOLA card without borders: automatic conversion of cryptocurrency and fiat. Payment for tickets and hotels through the</p>
      </h3>
    </article>

    <article class="cardslider__filter" @click="next">
      <img class="cardslider__img" src="../assets/images/filter/filter.png" srcset="../assets/images/filter/filter@2x.png" alt="filter" />

      <h3>
        VOOLA technologes allow
        <p>Use of the VOOLA card is possible anywhere in the world where Mastercard, Visa, Union is supported pay.</p>
      </h3>
    </article>

    <article class="cardslider__buy" @click="prev">
      <img class="cardslider__img" src="../assets/images/buy/buy.png" srcset="../assets/images/buy/buy@2x.png" alt="buy" />

      <h3>
        Shopping
        <p>Use of the VOOLA card when making purchases</p>
      </h3>
    </article>
  </section>
</template>

<script>
export default {
  data() {
    return {
      index: 0,
    }
  },
  methods: {
    next() {
      if (this.index === -728) {
        this.index = 0
      } else {
        this.index -= 264
      }
    },

    prev() {
      if (this.index === -244) {
      } else {
        this.index = 0
      }
    },
  },
}
</script>

<style lang="scss" scoped>
.cardslider {
  &__img {
    max-height: 92px;
    max-width: 92px;
  }

  &__bag,
  &__buy,
  &__filter {
    display: flex;
    position: absolute;

    h3 {
      margin: 0 40px 0 0;
    }

    p {
      margin: 10px 0 0 0;
    }
  }

  &__bag,
  &__buy {
    h3 {
      margin: 0 0 0 40px;
      max-width: 384px;
    }
  }

  &__bag {
    right: -35px;
    top: 180px;
    width: 624px;
  }

  &__buy {
    right: 208px;
    top: 570px;
    width: 440px;
  }

  &__filter {
    left: 80px;
    top: 305px;
    text-align: right;
    width: 570px;

    h3 {
      max-width: 340px;
    }

    img {
      order: 1;
    }
  }
}

@media only screen and(max-width:740px) {
  .cardslider {
    display: flex;
    transition: margin-left 0.7s ease-in-out;
    width: 100%;

    &__filter {
      text-align: left;

      img {
        order: 0;
      }
    }
    &__bag,
    &__buy,
    &__filter {
      background: rgba(255, 255, 255, 0.352);
      backdrop-filter: blur(6px);
      border-radius: 28px;
      display: flex;
      flex-direction: column;
      margin: 0 10px;
      min-width: 244px;
      padding: 20px;
      position: static;
      box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.01), 0px 8px 18px rgba(0, 0, 0, 0.02);

      img {
        width: 60px;
      }

      h3 {
        font-size: 19px;
        margin: 10px 0 0 0;
      }

      p {
        font-size: 15px;
        margin: 10px 0 0 0;
      }
    }
  }
}
</style>
