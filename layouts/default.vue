<template>
  <section id="app">
    <Header />
    <Nuxt />
    <Footer />
  </section>
</template>
<script>
import Header from './../components/Header'
import Footer from './../components/Footer'
export default {
  components: {
    Header,
    Footer
  }
}
</script>
<style lang="scss">
:root {
  --fontSize: .52085vw;
}
@font-face {
  font-family: 'ZenTokyo';
  src: local("ZenTokyo"),
  url(./assets/fonts/ZenTokyoZoo-Regular.ttf) format('truetype');
}
@font-face {
  font-family: 'Raleway-Bold';
  src: local("Raleway-Bold"),
  url(./assets/fonts/Raleway-Bold.ttf) format('truetype');
}
@font-face {
  font-family: 'Raleway-Italic';
  src: local("Raleway-Italic"),
  url(./assets/fonts/Raleway-Italic.ttf) format('truetype');
}
@font-face {
  font-family: 'Raleway-Light';
  src: local("Raleway-Light"),
  url(./assets/fonts/Raleway-Light.ttf) format('truetype');
}
@font-face {
  font-family: 'Raleway-Medium';
  src: local("Raleway-Medium"),
  url(./assets/fonts/Raleway-Medium.ttf) format('truetype');
}
@font-face {
  font-family: 'Raleway-Regular';
  src: local("Raleway-Regular"),
  url(./assets/fonts/Raleway-Regular.ttf) format('truetype');
}
body,html {
  margin: 0;
  padding: 0;
  font-family: Raleway-Regular;
  font-style: normal;
  overflow-x: hidden;
  font-size: var(--fontSize);
  scroll-behavior: smooth;
  -webkit-overflow-scrolling: touch;
  background: $default;
}
h1,h2,h3,h4,h5,h6,p,a,span {
  color: $white;
  margin: 0;
}
p,a {
  font-size: 1.8rem;
  text-decoration: none;
}
li {
  list-style: none;
}
ul {
  padding: 0;
}
.container {
  width: 150rem;
  margin: 0 auto;
}
.button__light {
  width: 22rem;
  height: 6rem;
  background: $white;
  color: $default;
  border: none;
  border-radius: 1rem;
  cursor: pointer;
  transition: .4s;
  &:hover {
    background: $brown;
    color: $white;
  }
}
@media screen and (max-width: 460px) {
  :root {
    --fontSize: 2.778vw;
  }
  .container {
    margin: 0;
    width: 36rem;
  }
}
</style>
