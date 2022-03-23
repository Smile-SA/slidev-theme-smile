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
      <div class="two-columns-demo__col-right col-right" :class="props.class">
        <slot name="right" />
      </div>
    </div>
  </div>
</template>
