<template>
  <section class="wallet">
    <img src="../assets/images/mobile/iPhone-24.png" srcset="../assets/images/mobile/iPhone-24@2x.png" alt="iPhone" />

    <article class="wallet__item">
      <h2>
        Wallet App
        <p>Securely store cryptocurrencies on your Android and Apple devices with VOOLA Gives you confidence that your digital assets are safe</p>
      </h2>
      <img src="../assets/images/mobile/iPhone-24.png" srcset="../assets/images/mobile/iPhone-24@2x.png" alt="iPhone" />
      <button @click="change">{{ title }}</button>
    </article>
  </section>
</template>

<script>
export default {
  data() {
    return {
      title: 'Download App',
    }
  },
  methods: {
    change() {
      this.title = 'Coming Soon'
    },
  },
}
</script>

<style lang="scss" scoped>
.wallet {
  align-items: center;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  margin: 0 auto;
  max-width: var(--scheme-max-width-wrapper);
  padding: 20px;

  img {
    filter: drop-shadow(-14px 16px 28px rgba(0, 0, 0, 0.04)) drop-shadow(-24px 36px 48px rgba(0, 0, 0, 0.1));
    margin: 0 134px 0 0;
    max-width: 252px;
  }

  &__item {
    max-width: 437px;

    img {
      display: none;
    }

    h2 {
      p {
        margin: 40px 0 40px 0;
      }
    }

    button {
      height: 60px;
      margin-top: 40px;
      width: 280px;
    }
  }
}

@media only screen and(max-width: 863px) {
  .wallet {
    text-align: center;

    h2 {
      font-size: 28px;

      p {
        font-size: 16px;
        margin: 20px 0 40px 0;
      }
    }

    img {
      display: none;
    }

    &__item {
      img {
        display: block;
        margin: 0 auto;
      }
    }
  }
}
</style>
