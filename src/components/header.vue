<template>
  <header class="header">
    <!-- Logo -->
    <div class="logo-container">
      <img src="public/logo.png" alt="Logo du site" class="logo" />
      <h1>App Météo</h1>
    </div>

    <!-- Navigation -->
    <nav class="nav">
      <RouterLink to="/">Accueil</RouterLink>
      <RouterLink to="/about">À propos</RouterLink>
    </nav>
  </header>
</template>

<script setup>

import logo from '@/public/logo.png'
</script>

<style scoped>
.header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  background-color: #1e1e2f;
  color: white;
  padding: 10px 30px;
  box-shadow: 0 2px 5px rgba(0,0,0,0.2);
}

.logo-container {
  display: flex;
  align-items: center;
  gap: 10px;
}

.logo {
  width: 50px;
  height: 50px;
  object-fit: contain;
}

.nav {
  display: flex;
  gap: 20px;
}

.nav a {
  color: white;
  text-decoration: none;
  font-weight: bold;
}


</style>
