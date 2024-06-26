<template>
  <div class="font-mono  text-gray-600">
    <div class="mx-auto mt-10 grid max-w-2xl grid-cols-1 gap-x-8 gap-y-16 border-t border-gray-200 pt-10 sm:mt-16 sm:pt-16 lg:mx-0 lg:max-w-none lg:grid-cols-3"
    ></div>
    <h2 class="text-4xl text-center font-bold max-md:text-xl">Tijan <span class="text-gray-500">Manandhar</span></h2>
    <div class="flex flex-row max-md:flex-col max-md:mt-5 mt-20">
      <div
          class="max-md:w-full lg:w-2/3 md:px-10 max-lg:order-2 py-10 items-items-center text-center lg:text-2xl lg:leading-10">
        <p>📸 Hi! I’m Tijan Manandhar, a web developer who dances with code and captures moments through a camera
          lens.</p>
        <p>🎨 When I’m not crafting backends with Node.js and PHP, I’m busy painting user interfaces with Vue.js and
          React.</p>
        <p>🎵 Music fuels my creativity, and hiking clears my cache—essential for a balanced developer life.</p>
        <p>🚀 Connect with me to build something awesome together!</p>
        <p>👩‍💻 A proud GDG Canberra co-organizer.</p>
      </div>
      <div class="justify-center lg:w-1/3 max-lg:order-1 max-md:w-full px-10 flex flex-col justify-center">
        <img class="rounded-full" src="/img/portrait.webp"/>
      </div>

    </div>

  </div>
</template>

<script setup>

useHead({
  title: 'About Me | Tijan Manandhar',
});

</script>