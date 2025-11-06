<script setup>
import { RouterView } from "vue-router";
import FooterComponent from "./components/Footer.vue";
</script>

<template>
  <div class="page">
    <header></header>

    <main class="main">
      <RouterView />
    </main>

    <FooterComponent />
  </div>
</template>

<style scoped>
.page {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

.main {
  flex-grow: 1;
}
</style>
