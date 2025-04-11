<template>
        <button class="w-[227px] h-[60px] bg-secondary rounded-lg">
            {{title}} <i class="pi pi-arrow-right px-1" style="color: white; font-size: 0.7rem;"></i>
        </button>
</template>

<script setup lang="ts">
defineProps<{
  title?: string
}>()

</script>