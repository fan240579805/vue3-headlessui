<template>
  <h3 class="bg-red-400">vite app</h3>
  <div class="wrap">
    <div class="ele_Wrap">
      <h4 style="margin-bottom: 30px">element ui 区域</h4>
      <elementDemo />
    </div>
    <div class="headless_Wrap">
      <h4 style="margin-bottom: 30px">headless ui 区域</h4>
      <SwitchDemo />
      <asd></asd>
    </div>
  </div>
</template>

<script setup>
import SwitchDemo from "./components/SwitchDemo.vue";
import elementDemo from "./components/elementDemo.vue";
import asd from "./components/asd.vue";
// This starter template is using Vue 3 experimental <script setup> SFCs
// Check out https://github.com/vuejs/rfcs/blob/script-setup-2/active-rfcs/0000-script-setup.md
</script>

<style scoped>
h3 {
  text-align: center;
  color: #fff;
}
.wrap {
  width: 90vw;
  margin: 80px auto;
  display: flex;
  justify-content: space-between;
}
.headless_Wrap,
.ele_Wrap {
  width: 42vw;
  border: 1px solid #333;
  padding: 30px;
}
</style>
