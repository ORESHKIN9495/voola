<template>
  <section class="card">
    <article class="card__item">
      <img src="../assets/images/lock/Lock.png" srcset="../assets/images/lock/Lock@2x.png" alt="lock" />

      <h3>Bypass cryptocurrency ban</h3>

      <p>The functionality allows you to bypass the ban on buy and sell cryptocurrencies</p>
    </article>

    <article class="card__item">
      <img src="../assets/images/wallet/Wallet.png" srcset="../assets/images/wallet/Wallet@2x.png" alt="wallet" />

      <h3>Buy/Sell cryptocurrency</h3>

      <p>Just a few clicks, you can buy Bitcoin or any other crypto coins</p>
    </article>

    <article class="card__item">
      <img src="../assets/images/key/Password.png" srcset="../assets/images/key/Password@2x.png" alt="key" />

      <h3>Favorable deposit in crypto</h3>

      <p>Invest your cryptocurrency at a favorable interest</p>
    </article>

    <article class="card__item">
      <img src="../assets/images/swap/Swap.png" srcset="../assets/images/swap/Swap@2x.png" alt="swap" />

      <h3>Cryptocurrency exchange</h3>

      <p>Cryptocurrency exchange</p>
    </article>

    <article class="card__item">
      <img src="../assets/images/call/Call.png" srcset="../assets/images/call/Call@2x.png" alt="call" />

      <h3>Mobile App</h3>

      <p>Only you have access to your wallet</p>
    </article>

    <article class="card__item">
      <img src="../assets/images/shield/Shield.png" srcset="../assets/images/shield/Shield@2x.png" alt="shield" />

      <h3>Reliable protection of your funds</h3>

      <p>Our crypto wallet provides reliable protection against fraudsters</p>
    </article>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.card {
  &__items {
    display: grid;
    gap: 20px;
    grid-template-columns: repeat(auto-fit, minmax(376px, 1fr));
    width: 100%;
  }

  &__item {
    background: rgb(255, 255, 255);
    border-radius: 28px;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.01), 0px 8px 18px rgba(0, 0, 0, 0.02);
    padding: 28px 32px;

    img {
      width: 44px;
      height: 44px;
      margin-bottom: 30px;
    }
  }
}
@media only screen and(max-width:575px) {
  .card {
    &__item {
      text-align: center;
      padding: 20px;

      h3 {
        margin: 0;
      }

      img {
        margin-bottom: 5px;
      }
    }
    &__items {
      gap: 12px;
      grid-template-columns: none;
    }

    &__logo {
      transform: rotate(90deg);

      img {
        width: 869px;
      }
    }
  }
}
</style>
