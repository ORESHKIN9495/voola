<template>
  <section class="cryptocurrency">
    <article class="cryptocurrency__item">
      <h2>
        Stable <span>NFT</span> cryptocurrency
        <p>
          We are leaders in the field of combining non-fungible NFT tokens and the world of fiat currencies. A breakthrough in the traditional financial system and a pioneer in
          NFTs using traditional currencies, Stable NFT tokens support and empower growing businesses and innovation in the blockchain space. Stable NFT tokens exist as digital
          tokens built on multiple blockchains. All Stable NFT tokens are 1:1 pegged to their respective fiat currency and are 100% backed by reserves. We publish a daily report on
          current total assets and reserves.<br /><br />
          Stable NFT tokens are virtual collectible gold coins with a denomination that move across the blockchain just as easily as other digital currencies, but are pegged to
          real currencies at a 1:1 ratio.
        </p>
      </h2>
      <img src="../assets/images/rectangle/rectangle.png" srcset="../assets/images/rectangle/rectangle@2x.png" alt="rectangle" />
    </article>

    <article class="cryptocurrency__item">
      <img src="../assets/images/spiral/spiral.png" srcset="../assets/images/spiral/spiral@2x.png" alt="spiral" />
      <h2>
        What are <span>Stable NFT</span> tokens and how do they work?
        <p>
          Stable NFT tokens are called stable NFT coins because they provide price stability as they are pegged to a fiat currency. This offers traders, sellers and funds a low
          volatility solution when exiting positions in the market. All Stable NFT tokens are 1:1 pegged to their respective fiat currency (e.g. $1T = $1) and are 100% backed by
          reserves. As a fully transparent company, we publish a report on current reserve assets.
        </p>
      </h2>
    </article>

    <article class="cryptocurrency__item">
      <h2>
        Where to store NFT?
        <p>
          VOOLA provides an easy and secure way to store all your Ethereum and BSC crypto collectibles. Your crypto-currency collectibles are securely secured on the blockchain and
          linked to a public address.
        </p>
      </h2>
      <img src="../assets/images/abstr/abstr.png" srcset="../assets/images/abstr/abstr@2x.png" alt="abstr gradient nft " />
    </article>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.cryptocurrency {
  margin: 0 auto;
  max-width: var(--scheme-max-width-wrapper);
  padding: 20px;

  &__item {
    align-items: center;
    display: flex;
    justify-content: space-between;

    span {
      font-weight: bold;
    }

    img {
      margin: 120px 0;
      max-width: 630px;
      width: 100%;
    }

    h2 {
      max-width: 547px;

      p {
        margin: 40px 0 0 0;
      }
    }

    &:nth-child(2) {
      img {
        max-width: 500px;
      }
    }
    &:last-child {
      img {
        margin: 120px 0 40px 0;
        max-width: 467px;
      }
    }
  }
}

@media only screen and(max-width: 1051px) {
  .cryptocurrency {
    &__item {
      flex-wrap: wrap;
      justify-content: center;

      h2 {
        max-width: 100%;
        font-size: 26px;
      }

      &:nth-child(2) {
        img {
          display: none;
        }
      }

      &:last-child {
        h2 {
          order: 1;
        }
      }
    }
  }
}
</style>
