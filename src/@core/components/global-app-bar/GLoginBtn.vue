<template>
  <BaseBtn :loading="loading" prepend-icon="$mdiAccount" @click="handler()">
    {{ userDisplayName }}
  </BaseBtn>
</template>

<script setup>
let loading = $ref(false)

let auth = useAuthStore()

let userDisplayName = computed(() =>
  auth.userDisplayName ? `Logout ${auth.userDisplayName}` : 'Login'
)

let handler = async () => {
  loading = true
  await auth.logout()
  loading = false
}
</script>
