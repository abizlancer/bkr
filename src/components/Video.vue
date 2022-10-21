<template>
  <section class="video">
    <img src="../assets/images/video-bg.png" alt="video">
    <article class="video__content">
      <div class="container">
        <div class="video__content--play">
          <img src="../assets/images/icons/crumbs-orange.svg" alt="crimbs">
          <div class="video--play-btn icon-play"></div>
        </div>
        <div class="video__content--title">
          <titles sub-title="Our Video" title="Story Behind Every Piece" />
        </div>
      </div>
    </article>
  </section>
</template>

<script>
import Titles from './Titles.vue'

export default {
  name: "Video",
  components: {
    Titles
  }
}
</script>