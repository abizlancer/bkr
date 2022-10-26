<template>
  <Navbar />
  <Header />
  <About />
  <Baked />
  <Video />
  <Products />
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Header from "./components/Header.vue";
import About from "./components/About.vue";
import Video from "./components/Video.vue";
import Products from "./components/products/Products.vue";
import Baked from "./components/baked/Baked.vue"

export default {
  name: 'App',
  components: {
    Navbar,
    Header,
    About,
    Baked,
    Video,
    Products,
  },
 
}
</script>

<style lang="scss">
  @import './assets/scss/main.scss';
</style>
