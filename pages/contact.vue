<script setup lang="ts">
useHead({
  title: 'My App',
  meta: [
    {name: 'contact', content: 'Contact with me to work with me.'}
  ],
  bodyAttrs: {
    class: 'test'
  },
  script: [{innerHTML: 'console.log(\'Hello world\')'}]
})

</script>

<template>
  <div>
    Contact me
  </div>
</template>