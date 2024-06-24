<template>
  <div class="font-mono">
    <div class="mx-auto mt-10 grid max-w-2xl grid-cols-1 gap-x-8 gap-y-16 border-t border-gray-200 pt-10 sm:mt-16 sm:pt-16 lg:mx-0 lg:max-w-none lg:grid-cols-3">
      <a :href="post.url" target="_blank" v-for="post in _posts" :key="post.id" class="flex max-w-xl flex-col items-start" v-if="_posts.length">
      <div class="image flex">
        <img :src="post.cover_image" alt="" v-if="post.cover_image">
        <img src="/blog_default.webp" alt="" v-if="!post.cover_image">
      </div>
        <div class="flex items-center gap-x-4 text-xs">
          <time :datetime="post.datetime" class="text-gray-500">{{ post.readable_publish_date }}</time>
        </div>
        <div class="group relative">
          <h3 class="mt-3 text-lg font-semibold leading-6 text-gray-900 group-hover:text-gray-600">
              {{ post.title }}
          </h3>
          <p class="mt-5 line-clamp-3 text-sm leading-6 text-gray-600">{{ post.description }}</p>
        </div>
      </a>
      <span v-if="!_posts.length">Loading</span>
    </div>
  </div>
</template>

<script setup>
import {useRouter} from "vue-router";

useHead({
  title: 'Blogs | Tijan Manandhar',
})

const router = useRouter()

let _posts = []
_posts = await $fetch('https://dev.to/api/articles?username=tijanmdr').catch((error) => error.data);
</script>