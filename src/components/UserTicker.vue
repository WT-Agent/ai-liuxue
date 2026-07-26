<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 139****2211 完成了英国 IC 计算机硕士 PS 个人陈述提炼"
  },
  {
    "text": "用户 186****9012 生成了美国哥大商业分析 SOP 目的陈述"
  },
  {
    "text": "用户 131****4490 完成了香港大学金融学推荐信专家框架"
  },
  {
    "text": "用户 158****7721 生成了低 GPA 逆袭爱丁堡大学解释信"
  },
  {
    "text": "用户 173****3389 取得了卡耐基梅隆大学人工智能全奖直博 PS 策划"
  }
]);
</script>
