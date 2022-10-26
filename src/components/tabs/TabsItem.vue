<template>
  <article>
    <h4>{{ item.title }}</h4>
    <p>{{ item.text }}</p>
  </article>
</template>

<script>
export default {
  name: "TabsItem",
  props: ["item"],
}
</script>