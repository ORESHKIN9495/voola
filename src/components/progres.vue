<template>
  <section class="progress">
    <h2>
      Assets and blockchains supported by VOOLA
      <p>Listing in progress….</p>
    </h2>
    <img src="../assets/images/progress/progress.png" srcset="../assets/images/progress/progress@2x.png" alt="progress" />
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.progress {
  max-width: var(--scheme-max-width-wrapper);
  margin: 80px auto;
  text-align: center;
  padding: 20px;
  h2 {
    font-size: 44px;
    color: var(--scheme-v2);
    p {
      font-size: 20px;
      color: var(--scheme-v3);
      margin: 40px 0 0 0;
    }
  }
  img {
    max-width: 800px;
    width: 100%;
  }
}
</style>
