<template>
  <div class="h-screen p-5 bg-white">
    <NuxtLayout>
      <Header/>
      <NuxtLoadingIndicator/>
      <NuxtPage class="min-h-screen"/>
      <Footer/>
    </NuxtLayout>
  </div>
</template>
<script setup lang="ts">
useHead
({
  title: 'Tijan Manandhar',
  meta: [
    {
      name: 'description', content: 'Hi I am Tijan Manandhar and you can contact me to work with me'
    }
  ],
  bodyAttrs: {
    class: 'test'
  },
  script: [{
    innerHTML: 'console.log(\'To connect with me: https://linkedin.com/in/tijanmdr/\')'
  }]
})
import Header from "~/layouts/header.vue";
import Footer from "~/layouts/footer.vue";
</script>