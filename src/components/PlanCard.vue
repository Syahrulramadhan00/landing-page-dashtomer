<script setup lang="ts">
import { Benefits } from '@/models/Benefits';

defineProps<{
  title: string
  desc: string
  isPremium?: boolean
  price: string
  benefit: string[]
}>()
</script>

<template>
<div
:class="[
  'rounded-xl p-6 shadow-md transition-all duration-300 shrink-0 snap-center',
  'w-[472px] max-sm:w-[80vw] max-sm:max-w-[80vw]',
  isPremium
    ? 'bg-main text-white'
    : 'bg-white text-dark border border-gold'
]"
>

  <div class="flex flex-col items-start justify-start px-10 my-20">
      <div class="flex flex-col space-y-6">
          <h2 class="text-2xl font-semibold">{{ title }}</h2>
          <p
            :class="[
                'font-bold text-4xl',
                isPremium ? 'text-gold' : 'text-dark'
            ]"
            >
            {{ price }}
            </p>
          <p class="text-lg font-medium">{{ desc }}</p>
      </div>
      <div class="mt-4 flex flex-col gap-4">
        <div
            v-for="(benefit, index) in benefit"
            :key="index"
            class="flex items-center space-x-4"
        >
            <i class="pi pi-check-circle text-yellow-300 text-[18px]"></i>
            <p 
            :class="[
                'font-normal text-lg',
                isPremium ? 'text-white' : 'text-dark'
            ]"
            >
            {{ benefit }}</p>
        </div>
        </div>
  </div>
  </div>
</template>