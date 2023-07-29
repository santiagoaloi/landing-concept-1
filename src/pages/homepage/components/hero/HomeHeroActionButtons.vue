<template>
  <div class="mt-9">
    <VBtn :block="smAndDown" class="rounded-lg" color="primary" size="x-large"> Get a demo </VBtn>
    <VBtn
      :block="smAndDown"
      :class="[!smAndDown && 'ml-5', smAndDown && 'mt-5']"
      class="rounded-lg"
      size="x-large"
      variant="tonal"
    >
      Post a free job
    </VBtn>
  </div>
</template>
<script setup>
const { smAndDown } = useDisplay()
</script>
