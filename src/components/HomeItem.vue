<script setup>
import { defineProps } from 'vue';

defineProps({
  bg: {
    type: String,
    default: 'bg-gray-100', // This can be passed as a prop to the component
  },
});
</script>

<template>
  <div :class="bgClass" class="card">
    <slot></slot>
  </div>
</template>

<style>
/* Card Styles */
.card {
  padding: 1.5rem; /* Equivalent to p-6 */
  border-radius: 0.5rem; /* Equivalent to rounded-lg */
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); /* Equivalent to shadow-md */
}

/* Default Background Color */
.bg-gray-100 {
  background-color: #643b3b; /* Equivalent to bg-gray-100 */
}

/* Additional Background Classes */
.bg-white {
  background-color: white;
}

.bg-blue-100 {
  background-color: #644040;
}

.bg-green-100 {
  background-color: #614343;
}
</style>
