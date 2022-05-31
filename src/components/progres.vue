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
  margin: 80px auto;
  max-width: var(--scheme-max-width-wrapper);
  padding: 20px;
  text-align: center;

  p {
    color: var(--scheme-v3);
    margin: 40px 0 20px 0;
  }

  img {
    max-width: 800px;
    width: 100%;
  }
}

@media only screen and(max-width:740px) {
  .progress {
    h2 {
      font-size: 28px;
    }
  }
}
</style>
