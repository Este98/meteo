<script setup>
import { RouterLink } from 'vue-router'

const year = new Date().getFullYear()
</script>

<template>
  <footer class="bg-light py-3 mt-4 border-top">
    <div class="color-container">
      <nav aria-label="Footer navigation">
        <ul class="list-unstyled d-flex justify-content-center align-items-center gap-4 mb-0">
          <li>
            <RouterLink to="MentionsLegales" class="nav-link">Mentions légales</RouterLink>
          </li>
          <li>
            <RouterLink to="APropos" class="nav-link">À propos</RouterLink>
          </li>
        </ul>
      </nav>
    </div>
  </footer>
</template>

<style scoped>
.color-container {
  background-color: hsl(232 29% 44%);
  color: white;
  padding: 2rem;
  border-radius: 8px;

  /* ✅ Centrage horizontal ET vertical */
  display: flex;
  justify-content: center;
  align-items: center;
}

/* Style des liens */
.nav-link {
  color: white;
  text-decoration: none;
  transition: color 0.3s;
}

.nav-link:hover {
  text-decoration: underline;
  color: hsl(232 40% 80%);
}
</style>
