<template>
  <TestJsx />
  <p class="color-primary">{{ name }}</p>
  <div>
    <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="@/assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>
  <HelloWorld msg="Vite + Vue" />
</template>

<script setup>
import { ref } from 'vue'
import HelloWorld from '@/components/HelloWorld.vue'
import TestJsx from '@/components/TestJsx.jsx'

const name = ref('123123')
</script>

<style lang="scss" scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
.color-primary {
  background-color: $bg-color-primary;
}
</style>
