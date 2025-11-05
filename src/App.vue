<script setup>
  import { RouterView, RouterLink } from "vue-router";
  import FooterComponent from "./components/Footer.vue";
</script>

<template>
  <header>
  </header>

  <main>
    <RouterView />
  </main>
  <FooterComponent/>
</template>
