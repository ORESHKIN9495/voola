<template>
  <section class="hero">
    <article class="hero__title">
      <img src="../assets/images/logo/Vector.png" srcset="../assets/images/logo/Vector@2x.png" alt="logo" />

      <h1>VOOLA is one of the most secure <b>crypto wallets</b></h1>

      <p>Purchase, collection, storage, exchange of cryptocurrencies and NFTs. By joining the VOOLA project, you become a member of the global crypto project.</p>

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
  display: flex;
  color: var(--scheme-v2);
  max-width: var(--scheme-max-width-wrapper);
  padding: 32px;

  &__title {
    img {
      height: 60px;
      margin-top: 85px;
      width: 200px;
    }

    h1 {
      font-size: 56px;
      margin: 123px 0 40px 0;
      max-width: 640px;
    }

    p {
      max-width: 500px;
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

@media only screen and(max-width:784px) {
  .hero {
    justify-content: center;
    flex-wrap: wrap;

    &__title {
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;

      h1 {
        font-size: 28px;
      }
    }
  }
}
</style>
