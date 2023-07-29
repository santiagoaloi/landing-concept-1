<template>
  <div v-if="mdAndUp" style="margin-top: -110px; margin-right: -450px">
    <VImg height="650" src="/hero.png" />
  </div>
</template>

<script setup>
const { mdAndUp } = useDisplay()
</script>
