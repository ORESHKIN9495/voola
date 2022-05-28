<template>
  <section class="footer">
    <img src="../assets/images/footer_logo/footer_logo.png" srcset="../assets/images/footer_logo/footer_logo@2x.png" alt="logo" />
    <p>All rights reserved</p>
    <p>made by <a href="/"> roobinium.io</a></p>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.footer {
  display: flex;
  justify-content: space-around;
  align-items: center;
  font-size: 14px;
  height: 100px;
  background: #f4f7fc;

  img {
    width: 100px;
    height: 30px;
  }

  p {
    color: rgba(29, 28, 40, 0.5);
    &:last-child {
      color: var(--scheme-v4);
    }
  }
}
</style>
