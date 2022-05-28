<template>
  <section class="wallet">
    <img src="../assets/images/mobile/iPhone-24.png" srcset="../assets/images/mobile/iPhone-24@2x.png" alt="iPhone" />

    <article class="wallet__item">
      <h2>
        Wallet App
        <p>Securely store cryptocurrencies on your Android and Apple devices with VOOLA Gives you confidence that your digital assets are safe</p>
      </h2>
      <img src="../assets/images/mobile/iPhone-24.png" srcset="../assets/images/mobile/iPhone-24@2x.png" alt="iPhone" />
      <button>Download App</button>
    </article>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.wallet {
  margin: 0 auto;
  max-width: var(--scheme-max-width-wrapper);
  display: flex;
  justify-content: center;
  padding: 20px;
  align-items: center;
  flex-wrap: wrap;
  img {
    width: 100%;
    height: 502.99px;
    max-width: 252px;
    margin: 0 134px 0 0;
    filter: drop-shadow(-14px 16px 28px rgba(0, 0, 0, 0.04)) drop-shadow(-24px 36px 48px rgba(0, 0, 0, 0.1));
  }

  &__item {
    max-width: 437px;
    width: 100%;

    img {
      display: none;
    }
    h2 {
      font-size: 44px;
      color: var(--scheme-v2);
      p {
        color: var(--scheme-v4);
        margin: 40px 0 0 0;
        font-size: 20px;
      }
    }

    button {
      background: var(--scheme-v3);
      border-radius: 16px;
      box-shadow: 0px 13px 18px rgba(0, 0, 0, 0.03);
      color: #fff;
      height: 60px;
      margin: 98px 0 40px 0;
      width: 280px;
    }
  }
}

@media only screen and(max-width: 861px) {
  .wallet {
    text-align: center;
    img {
      display: none;
    }
    &__item {
      img {
        margin: 0 auto;
        display: block;
      }
    }
  }
}
</style>
