<template>
  <div>
    <el-switch
      v-model="value1"
      active-text="按月付费"
      inactive-text="按年付费"
    >
      <!-- 渲染不进去 -->
      <p>123</p>
    </el-switch>
  </div>
</template>
<script setup>
import { ref } from "vue";
const value1 = ref(true);
const value2 = ref(true);
</script>
<style>
.elg {
  background-color: red;
}
</style>
