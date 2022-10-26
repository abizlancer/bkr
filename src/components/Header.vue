<template>
  <header class="header">
    <article class="header__info header-item container">
      <div class="header__info--content">
        <img src="../assets/images/icons/crumbs.svg" alt="crumbs">
        <div class="header__info--content__text">
          <titles subTitle="Sience 1984" title="Fresh Bakery Every Day" />
          <p>Even the all-powerful Pointing has no control about the blind texts it is an almost.</p>
        </div>
      </div>
    </article>
    <img src="../assets/images/main-bg.png" class="header-item main-bg" alt="mainBg">
  </header>
</template>

<script>
import Titles from './Titles.vue'

export default {
  name: 'Header',
  components: {
    Titles
  },
}
</script>