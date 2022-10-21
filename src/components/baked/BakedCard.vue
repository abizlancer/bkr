<template >
  <article v-for="(item, key) in items" :key="key" class="baked-card">
    <img :src="item.borderImg" alt="baked-bg" class="baked-card__border" >
    <div class="baked-card__content">
      <img :src="item.img" alt="card svg">
      <h4>{{ item.cardTitle }}</h4>
      <p>{{ item.cardText }}</p>
    </div>
  </article>
</template>

<script>
export default {
  name: 'BakedCard',
  props: {
    items: {
      type: Array
    }
  }
}
</script>