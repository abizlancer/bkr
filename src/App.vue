<template>
  <Navbar />
  <Header />
  <Baked />
  <Video />
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Header from "./components/Header.vue";
import Video from "./components/Video.vue";
import Baked from "./components/baked/Baked.vue"

export default {
  name: 'App',
  components: {
    Navbar,
    Header,
    Baked,
    Video,
  },
 
}
</script>

<style lang="scss">
  @import './assets/scss/main.scss';
</style>
