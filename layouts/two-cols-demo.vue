<script setup lang="ts">
const props = defineProps({
  class: {
    type: String,
  },
})
</script>

<template>
  <div class="slidev-layout two-columns-demo">
    <slot />
    <div class="two-columns-demo__cols grid grid-cols-2">
      <div class="col-left" :class="props.class">
        <slot name="left" />
      </div>
      <div class="col-right" :class="props.class" ref="right">
        <slot name="right" />
      </div>
    </div>
  </div>
</template>

<style scoped>
.two-columns-demo {
  display: flex;
  flex-direction: column;
}
.two-columns-demo__cols {
  flex: 1;
}
.col-right {
  border-color: inherit;
  border-width: 1px;
  padding: 10px;
  position: relative;
  overflow: auto;
}
</style>
