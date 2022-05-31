<template>
  <section class="footer">
    <div class="footer__wrapper">
      <img src="../assets/images/footer_logo/footer_logo.png" srcset="../assets/images/footer_logo/footer_logo@2x.png" alt="logo" />

      <p>All rights reserved</p>

      <p>made by <a href="/"> roobinium.io</a></p>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.footer {
  background: var(--scheme-v6);

  &__wrapper {
    align-items: center;
    display: flex;
    justify-content: space-between;
    margin: 0 auto;
    max-width: var(--scheme-max-width-wrapper);
    padding: 34px;
  }

  img {
    height: 30px;
    width: 100px;
  }

  p {
    color: var(--scheme-v5);

    &:last-child {
      color: var(--scheme-v4);
    }
  }
}

@media only screen and(max-width: 500px) {
  .footer {
    &__wrapper {
      flex-direction: column;
    }

    p {
      margin: 34px;

      &:last-child {
        margin: 0;
      }
    }
  }
}
</style>
