<script setup lang="ts">
import FooterMenu from './components/FooterMenu.vue'
import MainContent from './components/MainContent.vue'
import NavMenu from './components/NavMenu.vue'
</script>

<template>
  <header>
    <NavMenu />
  </header>

  <main>
    <MainContent />
  </main>

  <footer>
    <FooterMenu />
  </footer>
</template>

<style scoped>
header {
  position: sticky;
  top: 0;
  background-color: black;
  z-index: 999;
}
</style>
