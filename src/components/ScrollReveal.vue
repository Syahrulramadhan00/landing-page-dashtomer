<!-- components/ScrollReveal.vue -->
<template>
    <div
      ref="el"
      :class="['transition-all duration-700 ease-in-out', inView ? enterClass : exitClass]"
    >
      <slot />
    </div>
  </template>
  
  <script setup lang="ts">
  import { ref, onMounted, onUnmounted } from 'vue';
  
  const props = defineProps<{
    enterClass?: string;
    exitClass?: string;
  }>();
  
  const el = ref<HTMLElement | null>(null);
  const inView = ref(false);
  
  let observer: IntersectionObserver;
  
  onMounted(() => {
    observer = new IntersectionObserver(
      ([entry]) => {
        if (entry.isIntersecting) {
          inView.value = true;
          observer.unobserve(entry.target); // Remove if you want it only once
        }
      },
      {
        threshold: 0.2,
      }
    );
    if (el.value) observer.observe(el.value);
  });
  
  onUnmounted(() => {
    if (el.value) observer.unobserve(el.value);
  });
  </script>
  