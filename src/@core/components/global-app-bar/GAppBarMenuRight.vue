<template>
  <div v-if="mdAndUp">
    <div class="d-flex gap-2">
      <VBtn class="rounded-lg" color="accent-button" size="large" variant="elevated">
        Resources
      </VBtn>

      <VBtn class="rounded-lg" color="accent-button" size="large" variant="elevated">
        <VIcon color="accent-button-icon" icon="$mdiWeb" start> </VIcon>English
      </VBtn>

      <VBtn class="rounded-lg" color="accent-button" size="large" variant="elevated">
        <VIcon color="accent-button-icon" icon="$mdiAccountOutline" start> </VIcon>
        Login
      </VBtn>

      <VBtn class="rounded-lg" color="primary" size="large" variant="elevated"> Get a demo </VBtn>
    </div>
  </div>
  <VBtn v-else icon="$mdiMenu" size="small" />
</template>

<script setup>
const { mdAndUp } = useDisplay()
</script>
