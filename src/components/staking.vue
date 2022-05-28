<template>
  <section class="staking">
    <article class="staking__item">
      <h2>
        What is cryptocurrencies staking?
        <p>
          All blockchains have one feature: all transactions must be verified. Proof-of-Stake (PoS) is one of the mechanisms that has several verification variations of its own, as
          well as some hybrid models. For simplicity, we will call this staking. By staking coins, you get the opportunity to vote and earn income. This is similar to if you
          receive interest for keeping money in a bank account or providing it to a bank for investment. This system assumes a guaranteed income and a predictable source of income.
        </p>
      </h2>
      <img src="../assets/images/graph/graph.png" srcset="../assets/images/graph/graph@2x.png" alt="graph" />
    </article>

    <article class="staking__item">
      <img src="../assets/images/crystal/crystal.png" srcset="../assets/images/crystal/crystal@2x.png" alt="crystals" />
      <h2>
        Acquisition of NFT
        <p>
          Stable NFT tokens are called stable NFT coins because they provide price stability as they are pegged to a fiat currency. This offers traders, sellers and funds a low
          volatility solution when exiting positions in the market. All Stable NFT tokens are 1:1 pegged to their respective fiat currency (e.g. $1T = $1) and are 100% backed by
          reserves. As a fully transparent company, we publish a report on current reserve assets.<br /><br />
          The payment process using this virtual currency takes place in several stages. First, you need to enter the data from "Voolla Walet". After that, the money is debited
          from the buyer's account, and a payment receipt is sent to the email. If the payment on the website is in automatic mode, the order status changes to "Paid".
        </p>
      </h2>
    </article>

    <article class="staking__item">
      <h2>
        Crypto Voucher
        <p>
          "Crypto Voucher" is a payment system that simplifies the possibility of buying cryptocurrencies. A huge number of ways to purchase a Voucher makes the platform accessible
          to citizens of many countries. The following methods are offered for buying a Voucher:
        </p>
        <span>
          <img src="../assets/images/purchase/purchase.png" srcset="../assets/images/purchase/purchase@2x.png" alt="purchase" />
          <p>Purchase of a Voucher in terminals located in public places</p>
        </span>
        <span>
          <img src="../assets/images/mobilephone/mobilephone.png" srcset="../assets/images/mobilephone/mobilephone@2x.png" alt="mobile app" />
          <p>Purchase of a Voucher, through the mobile application "Viola Wallet"</p>
        </span>
        <p>
          Crypto Voucher will save you time rather than paying with bank cards. This payment system offers the cheapest way to buy cryptocurrencies, guaranteeing reliability and
          security. No matter how you bought Crypto Voucher, you can buy, exchange and make transactions with cryptocurrency in an instant!
        </p>
      </h2>
      <img src="../assets/images/voucher/voucher.png" srcset="../assets/images/voucher/voucher@2x.png" alt="voucher" />
    </article>

    <article class="staking__item">
      <img src="../assets/images/market/market.png" srcset="../assets/images/market/market@2x.png" alt="marketplace " />
      <h2>
        AR NFT Marketplace
        <p>
          NFT have 2D & 3D types and used in different industries: In Voola marketplace you can find all of this types NFT. You can see digital assets at home before actually
          purchasing them, use web-browser and look at your own NFT in AR device. Thanks to AR, you can associate the work you are viewing with the conditions of your environment,
          and you can explore new experiences with sound, visual, or other virtual effects. All procceses are automatical with simple interface and all you need is two clicks to
          make a purchase with a low fees.
        </p>
      </h2>
    </article>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.staking {
  max-width: var(--scheme-max-width-wrapper);
  margin: 0 auto;
  p {
    font-size: 20px;
  }
  h2 {
    font-size: 44px;
  }

  &__item {
    display: flex;
    justify-content: space-between;

    padding: 20px;
    align-items: center;

    img {
      max-width: 500px;
      max-height: 500px;
      width: 100%;
      height: 100%;
    }
    h2 {
      max-width: 600px;
      color: var(--scheme-v2);
      span {
        display: flex;
        align-items: center;

        img {
          width: 72px;
          height: 100%;
        }
        p {
          color: var(--scheme-v2);
          margin: 0 0 0 20px;
        }
      }

      p {
        margin: 40px 0;
        color: var(--scheme-v4);
        font-size: 20px;
      }
    }
    &:nth-child(2) {
      img {
        max-width: 533.5px;
        height: 100%;
      }
    }
    &:nth-child(3) {
      img {
        max-width: 625px;
        height: 100%;
      }
    }
    &:last-child {
      img {
        max-width: 536px;
        max-height: 760px;
        height: 100%;
      }
    }
  }
}

@media only screen and(max-width: 1110px) {
  .staking {
    &__item {
      justify-content: center;
      flex-wrap: wrap;
      span {
        img {
          display: block;
        }
      }

      img {
        display: none;
      }
      h2 {
        max-width: 100%;
      }

      &:nth-child(2) {
        img {
          order: 2;
          display: block;
        }
      }
      &:last-child {
        display: none;
      }
    }
  }
}
</style>
