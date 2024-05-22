<script setup lang="ts">
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>

  <div class="container">
    <HelloWorld  />
  </div>
</template>

<style scoped>
.container{
  height: 100vh;
  width: 100vw;
  background-image: url('./assets/images/background-pattern-desktop.svg');
  background-repeat: no-repeat;

  display: flex;
  justify-content: center;

}
</style>
