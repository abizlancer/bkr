<template >
  <small class="sub-title">{{ subTitle }}</small>
  <h1 class="title">{{ title }}</h1>
</template>

<script>
export default {
  props: ["subTitle", "title"]
}
</script>