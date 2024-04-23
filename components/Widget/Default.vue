<script setup lang="ts">
const props = defineProps<{
  title?: string
  subtitle?: string
}>()
</script>
<template>
  <div class="rounded-lg p-5 bg-white overflow-x-inherit">
    <div class="flex justify-between items-center">
      <div class="flex flex-col gap-1">
        <h3 class="font-[Inter] text-lg font-bold text-left text-gray-700">{{ props.title }}</h3>
        <p v-if="props.subtitle" class="font-[Inter] text-sm text-gray-500 text-left">{{ props.subtitle }}</p>
      </div>
      <slot name="header-actions" />
    </div>

    <div class="py-2">
      <slot />
    </div>
  </div>
</template>
