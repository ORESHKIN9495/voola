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
  max-width: var(--scheme-max-width-wrapper);
  margin: 0 auto;

  &__item {
    display: flex;
    justify-content: space-between;

    padding: 20px;
    align-items: center;

    span {
      font-weight: bold;
    }

    img {
      max-width: 630px;
      max-height: 472px;
      width: 100%;
      height: 100%;
    }
    h2 {
      max-width: 547px;
      color: var(--scheme-v2);

      p {
        margin: 40px 0 0 0;
        color: var(--scheme-v4);
        font-size: 20px;
      }
    }
    &:nth-child(2) {
      img {
        max-width: 500px;
        height: 100%;
      }
    }
    &:last-child {
      img {
        max-width: 467px;
        max-height: 440px;
        height: 100%;
      }
    }
  }
}

@media only screen and(max-width: 1110px) {
  .cryptocurrency {
    &__item {
      h2 {
        max-width: 100%;
      }
      justify-content: center;
      flex-wrap: wrap;

      &:nth-child(2) {
        img {
          display: none;
        }
      }
    }
  }
}
</style>
