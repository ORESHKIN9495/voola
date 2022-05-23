<template>
  <main></main>
</template>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
:root {
  // project color palete
  --scheme-v1: #ffffff; // primary scheme
  --scheme-v2: #ffffff;
  --scheme-v3: #ffffff;
  --scheme-v4: #ffffff;

  // project font-family
  --scheme-font: 'Helvetica', sans-serif;
  --scheme-h: 46px;
  --scheme-m: 32px;
  --scheme-s: 18px;

  // project default template width
  --scheme-max-width: 1280px; // desktop
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
}

body {
  background: var(--scheme-v2);
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
}

h1,
h2,
h3,
h4,
h5 {
  font-weight: 300;
  margin: 0;
}

h1 {
  font: 300 var(--scheme-h) / 1.42 var(--scheme-font);
  margin: 8rem 0 2rem;
}

h2 {
  font: 300 var(--scheme-m) / 1.42 var(--scheme-font);
  margin: 0 0 2rem;
}

h3 {
  font: 400 var(--scheme-s) / 1.42 var(--scheme-font);
  margin: 0 0 1rem;
}

a {
  color: inherit;
  text-decoration: none;
}

b {
  font-weight: 400;
}

p {
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
  background: none;
  border: none;
  box-shadow: none;

  font: var(--scheme-font);

  margin: 0;
  outline: none;
  padding: 0;
}
</style>
