<template>
  <VScrollYReverseTransition hide-on-leave>
    <VCard
      :key="route.name"
      :border="false"
      :class="[justifyCenter, fillHeight]"
      class="elevation-0 rounded-0 d-flex flex-column align-center bg-transparent px-8"
      min-height="100%"
    >
      <div :class="[hideOverflow, 'w-100 h-100 p-2']" :style="{ ...width }">
        <slot />
      </div>
    </VCard>
  </VScrollYReverseTransition>
</template>

<script setup>
/* Returns the current route location.*/
const route = useRoute()

const justifyCenter = computed(() => route.meta.justifyCenter && 'justify-center')
const fillHeight = computed(() => route.meta.fillHeight && 'fill-height')
const hideOverflow = computed(() => (route.meta.hideOverflow ? 'overflow-hidden' : 'overflow-auto'))
const width = computed(() => ({
  'max-width': route.meta.containerWidth || '1300px'
}))
</script>
