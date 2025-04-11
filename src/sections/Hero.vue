<script setup lang="ts">
import ButtonTry from '@/components/ButtonTry.vue';

</script>

<template>
    <div
      class="w-full py-12 md:py-2 h-[656px] 9xl:h-[829px] bg-main bg-no-repeat bg-center bg-[length:auto] overflow-hidden"
      style="background-image: url('/src/assets/dna.svg');"
    >
      <div class="flex flex-col md:flex-row items-center w-full h-full">
        <!-- Left Content -->
        <div class="w-full md:w-1/2 px-8 text-white font-inter text-center md:text-left">
          <h1 class="font-bold text-[40px] md:text-[54px] half7xl:text-[64px]">Get More Done with whitepace</h1>
          <p class="text-lg py-4">
            Project management software that enables your teams to collaborate, plan, analyze and manage everyday tasks
          </p>
          <div class="py-6">
            <ButtonTry title="Try Whitespace free" />
          </div>
        </div>
  
            <!-- Right Image -->
            <div class="flex max-w-full w-11/12 md:w-3/4 h-[300px] md:h-[71%] overflow-hidden mt-8 md:mt-0 justify-center mx-auto">
            <img 
                src="https://img.freepik.com/free-photo/group-people-working-out-business-plan-office_1303-15773.jpg?t=st=1744210723~exp=1744214323~hmac=3f4dde34c68be5b32a9a0dd22cf35b01eb17912dc504395d819f1cf939b57365&w=1380" 
                class="w-11/12 h-full object-cover object-left-top"
            />
            </div>

      </div>
    </div>
  </template>
  