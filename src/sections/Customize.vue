<script setup lang="ts">
import ButtonTry from '@/components/ButtonTry.vue';

</script>

<template>
    <div class="w-full max-md:py-32 space-y-25 min-h-[600px] flex flex-col justify-center items-center bg-main">
        <div class="flex flex-col md:flex-row w-full h-auto md:h-[448px] items-center gap-8">
          <!-- Left Content (40%) -->
          <div class="w-full md:w-[40%] h-full px-6 md:px-8 text-white font-inter text-center md:text-left flex flex-col justify-center">
            <div class="flex flex-col w-full space-y-6 max-w-[710px] mx-auto">
              <h1 class="font-bold text-[40px] md:text-[54px] half7xl:text-[72px] leading-tight">
                Use as
                <a
                  class="py-2 md:py-3 bg-no-repeat overflow-visible bg-[length:100%] bg-[bottom_right_-2rem]"
                  style="background-image: url('/src/assets/mini_underline.svg');"
                >
                  Extension
                </a>
              </h1>
              <p class="text-lg">
                Use the web clipper extension, available on Chrome and Firefox, to save web pages or take screenshots as notes.
              </p>
              <div class="pt-8 md:pt-20">
                <ButtonTry title="Let’s Go" class="text-white" />
              </div>
            </div>
          </div>
          <div class="w-full md:w-[60%] h-[300px] md:h-full flex justify-center items-center md:justify-start md:items-start mt-6 md:mt-0 px-4">
            <img
              src="https://img.freepik.com/free-photo/group-diverse-people-having-business-meeting_53876-25060.jpg?semt=ais_hybrid&w=740"
              class="w-11/12 h-full object-cover object-left-top"
            />
          </div>
        </div>
    </div>
    <div class="w-full max-md:py-32 space-y-25 min-h-[600px] flex flex-col justify-center items-center bg-white">
        <div class="flex flex-col-reverse md:flex-row w-full h-auto md:h-[448px] items-center gap-8">
            <div class="w-full md:w-[50%] h-[300px] md:h-full flex justify-center items-center md:justify-end md:items-end mt-6 md:mt-0 px-4">
            <img
              src="https://img.freepik.com/free-photo/group-diverse-people-having-business-meeting_53876-25060.jpg?semt=ais_hybrid&w=740"
              class="w-11/12 h-full object-cover object-left-top"
            />
          </div>
          <!-- Left Content (40%) -->
          <div class="w-full md:w-[60%] h-full px-6 md:px-8 text-dark font-inter text-center md:text-left flex flex-col justify-center">
            <div class="flex flex-col w-full space-y-6 max-w-[710px] mx-auto">
              <h1 class="font-bold text-[40px] md:text-[54px] half7xl:text-[72px] leading-tight">
                Customise it
                to <br class="hidden md:inline"/>
                <a
                  class="py-2 md:py-3 bg-no-repeat overflow-visible bg-[length:100%] bg-[bottom_right_-2rem]"
                  style="background-image: url('/src/assets/underline.svg');"
                >
                your needs
                </a>
              </h1>
              <p class="text-lg">
                Customise the app with plugins, custom themes and multiple text editors (Rich Text or Markdown). Or create your own scripts and plugins using the Extension API.
              </p>
              <div class="pt-8 md:pt-20">
                <ButtonTry title="Let’s Go" class="text-white" />
              </div>
            </div>
          </div>
        </div>
    </div>
</template>