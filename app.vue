<script setup lang="ts">
useSeoMeta({
  title: 'bilibili',
  description: '国内著名B站'
})
</script>

<template>
  <!-- <div>
    <NuxtWelcome />
  </div> -->
  <!-- <NuxtLink to="/">Home</NuxtLink>
  <NuxtLink to="/video">Video</NuxtLink> -->
  <!-- 缓存10级页面 -->
  <NuxtPage :keepalive="{ max: 10 }"></NuxtPage>
</template>

<style>
:root {
  --van-primary-color: #fb7299;
}
</style>