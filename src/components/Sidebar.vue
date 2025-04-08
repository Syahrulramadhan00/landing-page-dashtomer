
<template>
    <transition name="slide">
      <div v-if="isOpen" class="fixed inset-0 bg-transparent z-40" @click.self="closeSidebar">
        <div class="bg-main w-[250px] h-full p-6 text-white">
          <ul class="space-y-4 font-medium">
            <li class="flex justify-between items-center">
              Products <i class="pi pi-angle-down" style="color: white;"></i>
            </li>
            <li class="flex justify-between items-center">
              Solutions <i class="pi pi-angle-down" style="color: white;"></i>
            </li>
            <li class="flex justify-between items-center">
              Resources <i class="pi pi-angle-down" style="color: white;"></i>
            </li>
            <li class="flex justify-between items-center">
              Pricing <i class="pi pi-angle-down" style="color: white;"></i>
            </li>
          </ul>
          <div class="mt-8 space-y-4">
            <button class="w-full h-[50px] bg-gold text-main rounded-lg">
              Login
            </button>
            <button class="w-full h-[50px] bg-secondary rounded-lg text-white">
              Try Whitespace free <i class="pi pi-arrow-right px-1" style="font-size: 0.7rem;"></i>
            </button>
          </div>
        </div>
      </div>
    </transition>
  </template>
  
  <script setup>
  defineProps({ isOpen: Boolean })
  const emit = defineEmits(['close'])
  const closeSidebar = () => emit('close')
  </script>
  
  <style scoped>
  .slide-enter-active,
  .slide-leave-active {
    transition: all 0.3s ease;
  }
  .slide-enter-from {
    transform: translateX(-100%);
  }
  .slide-enter-to {
    transform: translateX(0);
  }
  .slide-leave-from {
    transform: translateX(0);
  }
  .slide-leave-to {
    transform: translateX(-100%);
  }
  </style>
  