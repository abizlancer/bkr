<template >
  <section class="baked process">
    <div class="baked--content process--content container">
      <titles subTitle="Our Process" title="How We Work" />
      <div class="baked__cards process__cards">
        <process-card :items="items" />
      </div>
    </div>
  </section>
</template>

<script>
import Titles from '../Titles.vue';
import ProcessCard from "./ProcessCard.vue";

export default {
    name: 'process',
    components: {
      Titles,
      ProcessCard
    },
    data() {
      return {
        items: [
          {
            img: 'src/assets/images/icons/love/card1.svg',
            borderImg: '/src/assets/images/love/item.png',
            cardTitle: 'Contact',
            cardText: 'Nothing the copy said could convince her and so it didn’t take long.'
          },
          {
            img: 'src/assets/images/icons/love/card1.svg',
            borderImg: '/src/assets/images/love/item.png',
            cardTitle: 'Baking',
            cardText: 'The copy said could convince her and so it didn’t take long.'
          },
          {
            img: 'src/assets/images/icons/love/card1.svg',
            borderImg: '/src/assets/images/love/item.png',
            cardTitle: 'Delivery',
            cardText: 'Nothing the copy said could convince her and so it didn’t take.'
          },
          {
            img: 'src/assets/images/icons/love/card1.svg',
            borderImg: '/src/assets/images/love/item.png',
            cardTitle: 'Tasty',
            cardText: 'Copy said could convince her and so it didn’t take long.'
          },
        ]
      }
    }
};
</script>