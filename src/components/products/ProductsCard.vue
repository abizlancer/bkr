<template>
  <article class="products__card">
    <slot></slot>
  </article>
</template>
<script>
export default {
  name: 'Products Card',
  props: {
    type: Array
  }
}
</script>