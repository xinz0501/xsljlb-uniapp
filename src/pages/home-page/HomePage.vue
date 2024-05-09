<!--
 * @Author: zhangxin
 * @Date: 2024-05-09 13:53:36
 * @LastEditors: zhangxin
 * @LastEditTime: 2024-05-09 16:52:06
 * @Description: 首页
-->
<template>
  <view class="content">
    <image class="logo" src="/static/logo.png"></image>
    <view class="text-area">
      <text class="title">{{ title }}</text>
    </view>
  </view>
</template>

<!-- <script>
export default {
  data() {
    return {
      title: 'Hello',
    }
  },
  onLoad() {},
  methods: {},
}
</script> -->

<script setup>
import { ref } from 'vue'

const title = ref('Hello')
</script>

<style>
.content {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.logo {
  height: 200rpx;
  width: 200rpx;
  margin-top: 200rpx;
  margin-left: auto;
  margin-right: auto;
  margin-bottom: 50rpx;
}

.text-area {
  display: flex;
  justify-content: center;
}

.title {
  font-size: 36rpx;
  color: #8f8f94;
}
</style>
