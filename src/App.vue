<script setup>
import { RouterView, RouterLink } from "vue-router";
import FooterComponent from "./components/Footer.vue";
import HeaderComponent from "./components/header.vue";
</script>

<template>
  <div id="app">
    <header>
      <HeaderComponent />
    </header>

    <main class="main">
      <RouterView />
    </main>

    <FooterComponent />
  </div>
</template>

<style scoped>
#app {
  display: flex;
  flex-direction: column;
  justify-content: center;
  min-height: 100vh;
}

.main {
  display: flex;
  flex-direction: column;
  flex: 1;
}
</style>
