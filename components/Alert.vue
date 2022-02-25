<script setup lang="ts">
  import { withDefaults } from 'vue';

  withDefaults(defineProps<{ type?: 'info' | 'warning' | 'error' }>(), { type: 'info' });
</script>

<style scoped>
  .alert {
    position: relative;
    display: flex;
    padding: 15px;
    font-size: 0.875rem;
    line-height: 1.25rem;
  }

  .alert::before {
    content: '';
    display: block;
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    opacity: 0.15;
    pointer-events: none;
  }

  .alert--info {
    color: var(--color-info);
  }

  .alert--info::before {
    background-color: var(--color-info);
  }

  .alert--warning {
    color: var(--color-warning);
  }

  .alert--warning::before {
    background-color: var(--color-warning);
  }

  .alert--error {
    color: var(--color-error);
  }

  .alert--error::before {
    background-color: var(--color-error);
  }

  .alert__icon {
    display: flex;
    align-items: center;
    padding: 0 25px 0 10px;
  }
</style>

<template>
  <div class="alert" :class="`alert--${type}`">
    <span class="alert__icon">
      <mdi-information-outline v-if="type == 'info'" />
      <mdi-alert-outline v-if="type == 'warning'" />
      <mdi-alert-circle-outline v-if="type == 'error'" />
    </span>
    <div>
      <slot></slot>
    </div>
  </div>
</template>