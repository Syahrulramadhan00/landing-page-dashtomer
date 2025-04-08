<!-- Hamburger.vue -->
<template>
    <div class="relative w-[42px] h-[42px] cursor-pointer z-50" @click="emit('toggle')">
      <span
        :class="[
          baseLine,
          'top-1/2 left-0',
          isOpen ? 'rotate-45' : '-translate-y-[10px]'
        ]"
      ></span>
      <span
        :class="[
          baseLine,
          'top-1/2 left-0',
          isOpen ? 'opacity-0' : ''
        ]"
      ></span>
      <span
        :class="[
          baseLine,
          'top-1/2 left-0',
          isOpen ? '-rotate-45' : 'translate-y-[10px]'
        ]"
      ></span>
    </div>
  </template>
  
  <script setup>
  import { computed } from 'vue'
  defineProps({ isOpen: Boolean })
  const emit = defineEmits(['toggle'])
  
  const baseLine = computed(() => 
    'absolute w-full h-[3px] bg-gray-300 rounded transition-all duration-300 origin-center'
  )
  </script>
  