<template>
  <button
    class="hover:TheShadow px-2 bg-white hover:border-primary hover:text-primary py-2 text-gray-400 transition-all border-gray-300 duration-200 border-2"
    :disable="IsDisabled"
    @click="$emit('onClick')"
  >
    <slot></slot>
  </button>
</template>

<script setup lang="ts">
defineProps({
  IsDisabled: {
    type: Boolean,
  },
});
</script>
