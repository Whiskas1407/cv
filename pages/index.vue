<template>
  <section class="app__home">
    <Home />
    <Skills />
    <Portfolio />
  </section>
</template>

<script>
import Home from './../components/Home'
import Skills from './../components/Skills'
import Portfolio from './../components/Portfolio'
export default {
  components: {
    Home,
    Skills,
    Portfolio
  }
}
</script>
<style lang="scss">

</style>
