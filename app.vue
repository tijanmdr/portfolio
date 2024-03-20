<template>
  <div class="h-screen p-5 bg-white">
    <NuxtLayout>
      <Header />
      <NuxtLoadingIndicator />
      <NuxtPage class="min-h-screen"/>
      <Footer />
    </NuxtLayout>
  </div>
</template>
<script setup lang="ts">
import Header from "~/layouts/header.vue";
import Footer from "~/layouts/footer.vue";
</script>