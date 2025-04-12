<script setup lang="ts">
import { ref } from 'vue'
import 'primeicons/primeicons.css'
import Hamburger from './Hamburger.vue'
import Sidebar from './Sidebar.vue'
import ButtonTry from './ButtonTry.vue'

const sidebarOpen = ref(false)
</script>

<template>
<div class="flex items-center w-full h-[92px] bg-main fixed top-0 left-0 z-50">
    <div class="flex items-center justify-between w-full 9xl:px-[220px] not-9xl:px-8 text-white">
      <div class="w-[191px] h-[34px] flex items-center justify-center shrink-0">
        <img src="/src/assets/icon.svg" class="w-full h-full object-contain" alt="" />
      </div>
      <div class="flex items-center justify-end space-x-12 not-half7xl:space-x-4 font-medium">
        <div class="flex items-center space-x-7 h-full not-half7xl:hidden ">
          <ul>Products<i class="pi pi-angle-down px-[10px]" style="color: white; font-size: 1rem;"></i></ul>
          <ul>Solutions<i class="pi pi-angle-down px-[10px]" style="color: white; font-size: 1rem;"></i></ul>
          <ul>Resources<i class="pi pi-angle-down px-[10px]" style="color: white; font-size: 1rem;"></i></ul>
          <ul>Pricing<i class="pi pi-angle-down px-[10px]" style="color: white; font-size: 1rem;"></i></ul>
        </div>
        <div class="flex items-center space-x-4 h-full not-md:hidden">
          <button class="w-[126px] h-[60px] bg-gold rounded-lg text-main">
            Login
          </button>
          <ButtonTry title="Try Whitespace free" />
        </div>
        <div class="flex items-center h-full half7xl:hidden">
          <Hamburger :isOpen="sidebarOpen" @toggle="sidebarOpen = !sidebarOpen" />
        </div>
      </div>
    </div>
    <Sidebar :isOpen="sidebarOpen" @close="sidebarOpen = false" />
  </div>
</template>
