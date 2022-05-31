<template>
  <main>
    <Hero />
    <Service />
    <Cryptocard />
    <Begin />
    <Cryptocurrency />
    <Progres />
    <Wallet />
    <Staking />
  </main>

  <footer>
    <Footer />
  </footer>
</template>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
@font-face {
  font-family: 'renner';
  src: url('../src/assets/fonts/renner/renner-light.otf');
}
:root {
  // project color palete
  --scheme-v1: #ffffff; // primary scheme
  --scheme-v2: #000000;
  --scheme-v3: #4e94d7;
  --scheme-v4: #62686d;
  --scheme-v5: rgba(29, 28, 40, 0.5);
  --scheme-v6: #f4f7fc;

  // project font-family
  --scheme-font: 'renner', sans-serif;
  --scheme-h: 56px;
  --scheme-m: 44px;
  --scheme-s: 24px;

  // project default template width
  --scheme-max-width: 1440px;
  --scheme-max-width-wrapper: 1300px; // desktop
  --scheme-min-width: 320px; // 5 SE

  // project default template height
  --scheme-min-height: 568px; // 5 SE

  // project default template gap
  --scheme-gap: 100px;

  // project ex. header & footer height
  --scheme-offset: 100px;
}

// project reset css
* {
  box-sizing: border-box;
}

html,
body {
  margin: 0;
  overflow-x: hidden;
}

body {
  background: var(--scheme-v1);
  color: var(--scheme-v1);

  font: 300 17px / 1.64 var(--scheme-font);

  // user-select: none;
  ::selection {
    background: var(--scheme-v3);
  }
  position: relative;
}

main,
section {
  position: relative;
  margin: 0 auto;

  // background: red;
}

h1,
h2,
h3,
h4,
h5 {
  color: var(--scheme-v2);
  font-weight: 300;
  margin: 0;
}

h1 {
  font: 300 var(--scheme-h) / 1.42 var(--scheme-font);
}

h2 {
  font: 300 var(--scheme-m) / 1.42 var(--scheme-font);
}

h3 {
  font: 400 var(--scheme-s) / 1.42 var(--scheme-font);
}

a {
  color: inherit;
  text-decoration: underline;
}

b {
  font-weight: 400;
}

p {
  color: var(--scheme-v4);
  font-size: 20px;
  margin: 0;
}

strong {
  font: inherit;
}

ul {
  margin: 0;
  padding: 0;

  li {
    list-style: none;
  }
}

figure {
  margin: 0;

  img {
    display: block;
    // object-fit: cover;
    width: 100%;
  }

  svg {
    vertical-align: middle;
  }
}

picture {
  img {
    width: 100%;
  }
}

input,
button {
  background: var(--scheme-v3);
  border: none;
  border-radius: 16px;
  box-shadow: none;
  color: var(--scheme-v1);

  font: var(--scheme-font);

  margin: 0;
  outline: none;
  padding: 0;
}

button {
  height: 60px;
  margin: 98px 0 40px 0;
  width: 280px;
}
</style>
