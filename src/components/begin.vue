<template>
  <section class="begin">
    <span class="begin__hand">
      <img src="../assets/images/phone/Phone.png" srcset="../assets/images/phone/Phone@2x.png" alt="hand" />
    </span>

    <div class="begin__items">
      <h2>Where to begin? With <b>simple steps</b></h2>

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
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: var(--scheme-v2);
  margin: var(--scheme-gap) auto;
  max-width: var(--scheme-max-width-wrapper);
  padding: 20px;

  &__hand {
    display: block;
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
    max-width: 366.33px;
    img {
      max-width: 366.33px;
    }
    &::before {
      background: red;
      content: '';
      position: absolute;
      width: 477.37px;
      height: 477.37px;
      background: linear-gradient(0deg, rgba(61, 118, 240, 0.26), rgba(61, 118, 240, 0.26)), radial-gradient(50% 50% at 50% 50%, #000000 0%, rgba(50, 66, 90, 0) 100%);
      opacity: 0.4;
      filter: blur(200px);
      border-radius: 317.5px;
      z-index: -1;
    }
  }

  &__items {
    width: 400px;

    h2 {
      margin: 0 0 60px 0;
    }
    img {
      max-width: 72px;

      margin: 0 20px 0 0;
    }
    p {
      color: var(--scheme-v2);
    }
  }
  &__item {
    display: flex;
    align-items: center;
    position: relative;
    margin: 20px 0;

    a {
      color: var(--scheme-v3);
    }

    &::after {
      content: '';
      background-image: url('../assets/images/Line.png');
      display: block;
      position: absolute;
      width: 24px;
      height: 2px;
      transform: rotate(90deg);
      margin: 95px 0px 0 25px;
    }

    &:last-child::after {
      content: none;
    }
  }
}

@media only screen and(max-width:784px) {
  .begin {
    &__hand {
      min-width: 281.92px;
      order: 1;
      margin: 120px 0 0 0;
      transform: rotate(-10deg);
      img {
        min-width: 281.92px;
      }
    }
    &__items {
      img {
        min-width: 56px;
      }
      h2 {
        min-width: 205px;
        font-size: 28px;
      }
    }
  }
}
</style>
