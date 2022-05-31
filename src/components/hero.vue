<template>
  <section class="hero">
    <article class="hero__title">
      <img src="../assets/images/logo/Vector.png" srcset="../assets/images/logo/Vector@2x.png" alt="logo" />

      <h1>VOOLA is one of the most secure <span>crypto wallets</span></h1>
      <p>Purchase, collection, storage, exchange of cryptocurrencies and NFTs. By joining the <span>VOOLA</span> project, you become a member of the global crypto project.</p>

      <button>Create Wallet</button>
    </article>

    <phone />
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.hero {
  align-items: center;
  display: flex;
  max-width: var(--scheme-max-width-wrapper);
  padding: 20px;

  &__title {
    img {
      width: 200px;
    }

    h1 {
      margin: 100px 0 40px 0;

      span {
        font-weight: bold;
      }
    }
    p {
      margin-bottom: 10px;
      max-width: 500px;
    }

    button {
      margin: 98px 0 40px 0;
    }
  }
}

@media only screen and(max-width:1080px) {
  .hero {
    flex-wrap: wrap;
    justify-content: center;

    &__title {
      text-align: center;
      margin-top: 35px;

      h1 {
        font-size: 28px;
        margin: 50px 0 20px 0;
      }
      p {
        font-size: 16px;
        margin: 0 auto;
      }

      button {
        margin: 40px 0 40px 0;
      }
    }
  }
}
</style>
