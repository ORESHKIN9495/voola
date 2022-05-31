<template>
  <section class="begin">
    <div class="begin__hand">
      <img src="../assets/images/phone/Phone.png" srcset="../assets/images/phone/Phone@2x.png" alt="hand" />
    </div>

    <div class="begin__items">
      <h2>Where to begin? With <span>simple steps</span></h2>

      <article class="begin__item">
        <img src="../assets/images/download/download.png" srcset="../assets/images/download/download@2x.png" alt="download" />

        <p><a href="/">Download</a> a wallet</p>
      </article>

      <article class="begin__item">
        <img src="../assets/images/create/create.png" srcset="../assets/images/create/create@2x.png" alt="create" />

        <p>Create your own wallet</p>
      </article>

      <article class="begin__item _it">
        <img src="../assets/images/receive/receive.png" srcset="../assets/images/receive/receive@2x.png" alt="receive" />

        <p>Receive</p>
      </article>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.begin {
  align-items: center;
  display: flex;
  justify-content: space-between;
  max-width: var(--scheme-max-width-wrapper);
  padding: 20px;

  &__hand {
    position: relative;
    img {
      max-width: 366px;
      width: 100%;
    }
    &::before {
      background: linear-gradient(0deg, rgba(61, 118, 240, 0.26), rgba(61, 118, 240, 0.26)), radial-gradient(50% 50% at 50% 50%, #000000 0%, rgba(50, 66, 90, 0) 100%);
      border-radius: 320px;
      content: '';
      filter: blur(200px);
      height: 600px;
      left: 0;
      max-width: 600px;
      opacity: 0.4;
      position: absolute;
      right: 0;
      top: 20px;
      z-index: -1;
    }
  }

  &__items {
    h2 {
      margin: 0 0 80px 0;
      max-width: 399px;

      span {
        font-weight: bold;
      }
    }

    img {
      margin: 0 20px 0 0;
      max-width: 72px;
    }

    p {
      color: var(--scheme-v2);
    }
  }

  &__item {
    align-items: center;
    display: flex;
    margin: 20px 0;
    position: relative;

    a {
      color: var(--scheme-v3);
    }

    &::after {
      background-image: url('../assets/images/Line.png');
      content: '';
      display: block;
      height: 2px;
      margin: 95px 0px 0 25px;
      position: absolute;
      transform: rotate(90deg);
      width: 24px;
    }

    &:last-child::after {
      content: none;
    }
  }
}

@media only screen and(max-width:784px) {
  .begin {
    &__hand {
      margin-top: 120px;
      order: 1;
      transform: rotate(-10deg);

      img {
        min-width: 280px;
      }
    }

    &__items {
      h2 {
        font-size: 27px;
        min-width: 188px;
      }
    }
  }
}
</style>
