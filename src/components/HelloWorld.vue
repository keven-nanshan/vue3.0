
<template>
  <h1>{{ msg }}</h1>

  <div class="card">
    <el-button type="warning" @click="count++">count is {{ count }}</el-button>
  </div>

  <el-row class="mb-4">
    <el-button>Default</el-button>
    <el-button type="primary">Primary</el-button>
    <el-button type="success">Success</el-button>
    <el-button type="info">Info</el-button>
    <el-button type="warning">Warning</el-button>
    <el-button type="danger">Danger</el-button>
  </el-row>
</template>
<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>
<style scoped>
.read-the-docs {
  color: #888;
}
</style>
