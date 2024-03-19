<template>
  <div>
    <NuxtLayout>
      <Header />
      <NuxtLoadingIndicator />
      <NuxtPage />
    </NuxtLayout>
  </div>
</template>
<script setup lang="ts">
import Header from "~/layouts/header.vue";
</script>