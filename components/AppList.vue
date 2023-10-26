<template>
      <NuxtLink class="v-card" :key="item.aid" :to="`/video/${item.bvid}`">
        <div class="card">
          <div class="card-img">
            <img class="pic" :src="item.pic" :alt="item.title" />
          </div>
          <div class="count">
            <span>
              <i class="iconfont icon_shipin_bofangshu"></i>
              {{ item.stat.view }}
            </span>
            <span>
              <i class="iconfont icon_shipin_danmushu"></i>
              {{ item.stat.danmaku }}
            </span>
          </div>
        </div>
        <!-- <p class="title">当你觉得扛不住的时候来看看这段视频</p> -->
        <p class="title">{{ item.title }}</p>
      </NuxtLink>
</template>

<script setup lang="ts">
import type { VideoTs } from '~/types/video';

  defineProps<{
    item: VideoTs
  }>()
</script>

<style scoped>

</style>