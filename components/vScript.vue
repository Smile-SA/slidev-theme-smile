<script setup>
import { h, onMounted, ref, useAttrs, useSlots } from 'vue';

const placeholderRef = ref();
const isOverview = ref();
const isMounted = ref();

function hasSomeParentTheClass(element, classname) {
  if (element.classList.contains(classname)) return true;
  return element.parentElement && hasSomeParentTheClass(element.parentElement, classname);
}

onMounted(() => {
  isOverview.value = hasSomeParentTheClass(placeholderRef.value, 'slides-overview');
  isMounted.value = true;
});

const attrs = useAttrs();
const slots = useSlots();

function renderPlaceholder() {
  return h('div', { ref: placeholderRef });
}

function renderScript() {
  if (slots.default) {
    return h('script', attrs, slots.default());
  }
}
</script>

<template>
  <renderPlaceholder v-if="!isMounted"></renderPlaceholder>
  <renderScript v-if="isMounted && !isOverview"></renderScript>
</template>
