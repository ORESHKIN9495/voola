<template>
  <section class="phone">
    <article class="phone__item">
      <img src="../assets/images/mobile/iPhone-13.png" srcset="../assets/images/mobile/iPhone-13@2x.png" alt="iPhone" />

      <img src="../assets/images/mobile/iPhone-25.png" srcset="../assets/images/mobile/iPhone-25@2x.png" alt="iPhone" />
    </article>

    <article class="phone__item">
      <img src="../assets/images/mobile/iPhone-24.png" srcset="../assets/images/mobile/iPhone-24@2x.png" alt="iPhone" />

      <img src="../assets/images/mobile/iPhone-26.png" srcset="../assets/images/mobile/iPhone-26@2x.png" alt="iPhone" />
    </article>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.phone {
  display: flex;

  &__item {
    display: flex;
    flex-direction: column;
    margin-top: -240px;
    margin-right: -20px;
    filter: drop-shadow(-14px 16px 28px rgba(0, 0, 0, 0.04)) drop-shadow(-24px 36px 48px rgba(0, 0, 0, 0.1));

    img {
      width: 252px;
      margin: 20px;
    }

    &:last-child {
      margin-top: -370px;
    }
  }
}

@media only screen and(max-width:1080px) {
  .phone {
    &__item {
      display: flex;
      flex-direction: row;
      margin: 0;
      order: 2;

      img {
        width: 192px;
      }

      &:last-child {
        margin: 0;
        order: 1;

        img:first-child {
          display: none;
        }
      }
    }
  }
}
</style>
