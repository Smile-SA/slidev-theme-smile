<script setup lang="ts">
  import { computed } from 'vue';
  
  const props = defineProps<{ class?: string, color?: 'primary' | 'secondary', icon: string }>();

  const style = computed(() => {
    if (props.color) {
      return { color: `var(--color-${props.color})` };
    }
    return {};
  });
</script>

<style scoped>
.icon {
  display: inline-block;
  width: 1em;
  height: 1em;
  stroke-width: 0;
  stroke: currentColor;
  fill: currentColor;
}
</style>

<template>
  <svg class="icon" :class="{ [props.class]: props.class, [`icon-${icon}`]: icon }" :style="style">
    <use :xlink:href="`#icon-${icon}`"></use>
  </svg>
</template>
