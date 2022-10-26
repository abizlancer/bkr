<template>
  <div class="tabs">
    <span>01</span>
    <div class="tabs--content">
      <tabs-controls />
      <div class="tabs--content__items">
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
  props: ["items"]
};
</script>
