<!--
 * @Author: weisheng
 * @Date: 2024-11-01 11:44:38
 * @LastEditTime: 2024-11-01 14:10:20
 * @LastEditors: weisheng
 * @Description:
 * @FilePath: \wot-demo\src\pages\index.vue
 * 记得注释
-->
<script setup lang="ts">
const timeRange = ref([])
function handleConfirm({ value }) {
  console.log(value)
}
</script>

<template>
  <view class="px-3 py-20 text-center">
    <view class="mb-4 text-xl text-gray-9">
      hi！你好。
    </view>

    <view class="text-2xl text-gray-9!">
      <wd-text custom-class="text-gray-9!" text="欢迎使用 Wot Design Uni！" />
    </view>
    <view>
      <wd-datetime-picker v-model="timeRange" label="日期选择" type="time" @confirm="handleConfirm" />
    </view>
  </view>
</template>

<style></style>

<route type="home" lang="json">
{
  "layout": "tabbar",
  "name": "home",
  "style": {
    "navigationBarTitleText": "home"
  }
}
</route>
