<script setup lang="ts">
import ButtonTry from '@/components/ButtonTry.vue';

</script>

<template>
    <div
      class="w-full max-md:py-32 space-y-25 min-h-[1370px] flex flex-col justify-center items-center bg-no-repeat bg-top-left bg-[length:auto] overflow-hidden bg-white"
      style="background-image: url('/src/assets/spiral.svg');"
    >
      <!-- Project Management Section Start -->
      <div class="flex flex-col md:flex-row w-full h-auto md:h-[448px] items-center gap-8">
        <!-- Left Content (40%) -->
        <div class="w-full md:w-[40%] h-full px-6 md:px-8 text-dark font-inter text-center md:text-left flex flex-col justify-center">
          <div class="flex flex-col w-full space-y-6 max-w-[710px] mx-auto">
            <h1 class="font-bold text-[40px] md:text-[54px] half7xl:text-[72px] leading-tight">
              Project <br class="hidden md:inline"/>
              <a
                class="py-5 md:py-7 bg-no-repeat overflow-visible bg-[length:100%] bg-[bottom_right_-2rem]"
                style="background-image: url('/src/assets/underline.svg');"
              >
                Management
              </a>
            </h1>
            <p class="text-lg">
              Images, videos, PDFs and audio files are supported. Create math expressions and diagrams directly from the app. Take photos with the mobile app and save them to a note.
            </p>
            <div class="pt-8 md:pt-20">
              <ButtonTry title="Get Started" class="text-white" />
            </div>
          </div>
        </div>
  
        <!-- Right Image (60%) -->
        <div class="w-full md:w-[60%] h-[300px] md:h-full flex justify-center items-center md:justify-start md:items-start mt-6 md:mt-0 px-4">
          <img
            src="https://img.freepik.com/free-photo/group-diverse-people-having-business-meeting_53876-25060.jpg?semt=ais_hybrid&w=740"
            class="w-11/12 h-full object-cover object-left-top"
          />
        </div>
      </div>
      <!-- Project Management Section End -->
  
      <!-- Work Together Section Start -->
      <div class="flex flex-col-reverse md:flex-row items-center w-full h-auto md:h-[491px] gap-8">
        <!-- Left Image -->
        <div class="w-full h-[300px] md:h-full md:w-[50%] flex items-center justify-center overflow-hidden">
          <img
            src="/src/assets/work.svg"
            class="max-w-full max-h-full object-contain"
          />
        </div>
  
        <!-- Right Text -->
        <div class="w-full md:w-[50%] flex justify-center md:justify-start items-center md:items-start px-6 md:px-8 py-10 md:py-0">
          <div class="w-full md:w-full h-full flex flex-col items-center md:items-start text-dark font-inter text-center md:text-left max-w-[710px] space-y-6">
            <h1 class="font-bold text-[40px] md:text-[54px] half7xl:text-[72px] leading-tight">
              Work
              <a
                class="py-5 md:py-2 bg-no-repeat bg-[length:100%] bg-[bottom_right_-2rem]"
                style="background-image: url('/src/assets/underline.svg');"
              >
                Together
              </a>
            </h1>
            <p class="text-lg">
                With whitepace, share your notes with your colleagues and collaborate on them.
You can also publish a note to the internet and share the URL with others.

            </p>
            <div class="pt-8 md:pt-20">
              <ButtonTry title="Try it now" class="text-white" />
            </div>
          </div>
        </div>
      </div>
      <!-- Work Together Section End -->
    </div>
  </template>
  
  