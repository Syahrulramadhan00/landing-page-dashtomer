<script setup lang="ts">
import PlanCard from '@/components/PlanCard.vue'
import { Benefits } from '@/models/Benefits'
</script>

<template>
  <div class="w-full min-h-[600px] bg-white flex flex-col items-center justify-start py-12 space-y-16">
    <!-- Heading Section -->
    <div class="text-center max-w-[979px] w-full px-4 space-y-6">
      <h1 class="font-bold text-[40px] md:text-[54px] leading-tight">
        Choose 
        <span
          class="py-2 bg-no-repeat bg-[length:100%] bg-[bottom_right_-2rem]"
          style="background-image: url('/public/underline.svg');"
        >
          Your Plan
        </span>
      </h1>
      <p class="text-lg">
        Whether you want to get organized, keep your personal life on track, or boost workplace productivity, Evernote has the right plan for you.
      </p>
    </div>

    <!-- Carousel Section -->
    <div class="w-full overflow-x-auto max-sm:scroll-smooth max-sm:snap-x max-sm:snap-mandatory px-4">
      <div class="flex flex-nowrap space-x-5 sm:justify-center sm:overflow-x-hidden px-2">
        <PlanCard
          price="$0"
          title="Free"
          desc="Capture ideas and find them quickly"
          :is-premium="false"
          :benefit="Benefits"
        />
        <PlanCard
          price="$11.99"
          title="Personal"
          desc="Keep home and family on track"
          :is-premium="true"
          :benefit="Benefits"
        />
        <PlanCard
          price="$49.99"
          title="Organization"
          desc="Collaborate across teams and workspaces"
          :is-premium="false"
          :benefit="Benefits"
        />
      </div>
    </div>
  </div>
</template>
