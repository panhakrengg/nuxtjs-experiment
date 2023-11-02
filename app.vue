<template>
  <div>
    <NuxtLayout>
      <NuxtPage />
    </NuxtLayout>
  </div>
</template>
<script setup lang="ts">
const color = ref("blue")
</script>
<style lang="scss">
h1 {
  color: v-bind(color);
}
</style>
