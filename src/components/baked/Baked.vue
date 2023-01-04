<template >
  <section class="baked">
    <div class="baked--content container">
      <titles subTitle="Our Features" title="Baked With Love" />
      <div class="baked__cards">
        <baked-card :items="items" />
      </div>
    </div>
  </section>
</template>

<script>
import Titles from "../Titles.vue";
import BakedCard from "./BakedCard.vue";

export default {
  name: 'Baked',
  components: {
    Titles,
    BakedCard
  },
  data() {
    return {
      items: [
        {
          img: 'src/assets/images/icons/love/card1.svg',
          borderImg: '/src/assets/images/love/item.png',
          cardTitle: 'Fresh',
          cardText: 'Nothing the copy said could convince her and so it didn’t take long.'
        },
        {
          img: '/src/assets/images/icons/love/card2.svg',
          borderImg: '/src/assets/images/love/item.png',
          cardTitle: 'Natural',
          cardText: 'Copy Writers ambushed her, made her drunk with Longe and Parole.'
        },
        {
          img: '/src/assets/images/icons/love/card3.svg',
          borderImg: '/src/assets/images/love/item.png',
          cardTitle: 'Tasty',
          cardText: 'And if she hasn\'t been rewritten, then they are still using her.'
        }
      ]
    }
  },
}
</script>