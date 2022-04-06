<script setup lang="ts">
const props = defineProps<{
  content?: string;
  filename?: string;
  type?: string;
}>();
const { content, filename = 'file', type = 'text/plain' } = props

function handleClick() {
  if (content) {
    const blob = new Blob([content], { type });
    const url = window.URL.createObjectURL(blob);
    const a = document.createElement('a');
    a.style.display = 'none';
    a.href = url;
    a.download = filename;
    document.body.appendChild(a);
    a.click();
    window.URL.revokeObjectURL(url);
  } else {
    const a = document.createElement('a');
    a.style.display = 'none';
    a.href = filename;
    a.download = filename;
    document.body.appendChild(a);
    a.click();
  }
}
</script>

<template>
  <button class="primary" @click="handleClick">
    <slot></slot>
  </button>
</template>
