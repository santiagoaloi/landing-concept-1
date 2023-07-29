<template>
  <div class="review-wrapper">
    <div v-for="(_, i) in 2" :key="_" class="py-5">
      <div class="flex space-x-1">
        <VRating :model-value="3 + i" density="compact" length="5" readonly size="small" />
      </div>

      <p class="review-numbers"><span class="font-bold">4.6</span> /5 - from 12k reviews</p>
      <GoogleTitle />
    </div>
  </div>
</template>

<style scoped>
.review-wrapper {
  @apply mt-6 lg:mt-10 grid grid-cols-2 gap-x-5
}

.review-numbers {
  @apply mt-3 text-sm text-gray-800 dark:text-gray-200
}
</style>
