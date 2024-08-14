<script setup>
import AppHeader from './components/AppHeader.vue'
import AppMain from './views/AppMain.vue'
</script>

<template>
  <div class="layout">
    <AppHeader />
    <router-view />
    <!--<Footer />-->
  </div>
</template>

<style scoped>
.layout {
  width: 100%;
  height: 100%;
}
</style>