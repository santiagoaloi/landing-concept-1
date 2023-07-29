<template>
  <div class="mt-n1 active-push-down-no-shadow flex" @click="router.push('/')">
    <VImg class="ml-6" src="/logo.png" width="145" />
  </div>
</template>
<script setup>
const router = useRouter()
</script>
