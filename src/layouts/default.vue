<script setup lang="ts">
const deviceStore = useDeviceStore()
onMounted(() => {
  deviceStore.statusBarHide()
})
</script>

<template>
  <main px-4 py-10 text="center gray-700 dark:gray-200" class="h-screen w-full">
    <RouterView />
    <TheFooter />
    <div mx-auto mt-5 text-center text-sm opacity-50>
      [Default Layout]
    </div>
  </main>
</template>
