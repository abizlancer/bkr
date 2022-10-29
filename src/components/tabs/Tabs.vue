<template>
  <div class="tabs">
    <div class="tabs--content">
      <tabs-controls />
      <div class="tabs--content__items">
        <span>{{ span }}</span>
        <tabs-item v-for="(item, key) in items" :key="key" :item="item" />
      </div>
    </div>
  </div>
</template>

<script>
import TabsControls from "./TabsControls.vue"
import TabsItem from "./TabsItem.vue"

export default {
  name: "Tabs",
  components: {
    TabsControls,
    TabsItem
  },
  props: ["items", "span"]
};
</script>
