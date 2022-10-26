<template>
  <section class="about container">
    <article class="about__images">
      <!-- <img src="../assets/images/icons/crumbs.svg"  class="about__images--crumbs about--crumb" alt="crumbs"> -->
      <div class="about__images--items">
        <img src="../assets/images/special/item1.png" alt="about-img">
        <img src="../assets/images/special/item2.png" alt="about-img">
      </div>
      <!-- <img src="../assets/images/icons/crumbs-big.svg" class="about__images--crumbs about--crumb-big" alt="crumbs"> -->
    </article>
    <article class="about__info">
      <titles subTitle="About Us" title="Baking Special Moments"/>
      <tabs :items="tabsItems" />
    </article>
  </section>
</template>

<script>
import Titles from './Titles.vue'
import Tabs from './tabs/Tabs.vue'

export default {
  name: "About",
  components: {
    Titles,
    Tabs,
  },
  data() {
    return {
      tabsItems: [
        {
          title: "Last view back",
          text: "She packed her seven versalia, put her initial into the belt and made herself on the way. When she reached the first hills of the Italic.",
        },
        {
          title: "On the skyline",
          text: "She packed her seven versalia, put her initial into the belt and made herself on the way. When she reached the first hills of the Italic.",
        },
        {
          title: "Pityful a rethoric",
          text: "She packed her seven versalia, put her initial into the belt and made herself on the way. When she reached the first hills of the Italic.",
        },
        {
          title: "On her way she",
          text: "She packed her seven versalia, put her initial into the belt and made herself on the way. When she reached the first hills of the Italic.",
        },
      ]
    }
  },
}
</script>