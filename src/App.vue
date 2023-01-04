<template>
  <Navbar />
  <Header />
  <About />
  <Baked />
  <Video />
  <Products />
  <Process />
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Header from "./components/Header.vue";
import About from "./components/About.vue";
import Video from "./components/Video.vue";
import Products from "./components/products/Products.vue";
import Baked from "./components/baked/Baked.vue"
import Process from "./components/process/Process.vue";

export default {
  name: 'App',
  components: {
    Navbar,
    Header,
    About,
    Baked,
    Video,
    Products,
    Process,
  },
 
}
</script>

<style lang="scss">
  @import './assets/scss/main.scss';
</style>
