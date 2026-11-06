<!-- src/App.vue -->
<script setup>
  import { ref } from 'vue'

  const count = ref(0)
  const inputText = ref('')
</script>

<template>
  <div style="padding: 20px;">
    <h1>测试页面”修改为“Vite HMR 完美生效！</h1>

    <!-- 测试状态 1：输入框内容 -->
    <p>
      输入测试文字：<input v-model="inputText" placeholder="..." />
    </p>

    <!-- 测试状态 2：响应式计数器 -->
    <p>
      点击次数：<button @click="count++">{{ count }}</button>
    </p>
  </div>
</template>
