<script setup>
import TheKeyboard from './components/TheKeyboard.vue'
import DisplayPanel from './components/DisplayPanel.vue'
</script>

<template>
  <main>
    <DisplayPanel />
    <TheKeyboard />
  </main>
</template>

<style>
main {
  margin: 0 auto;
}

#app {
  text-align: center;
  align-content: center;
  font-size: 24px;
  margin: 0 auto;
}

@media (min-width: 1024px) {
}
</style>
