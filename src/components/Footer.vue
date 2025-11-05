<script setup>
import { RouterLink } from 'vue-router'

const year = new Date().getFullYear()
</script>

<template>
  <footer class="bg-light py-3 mt-4 border-top">
    <div class="color-container">
      <nav aria-label="Footer navigation">
        <ul class="footer-links">
          <li>
            <RouterLink to="MentionsLegales" class="nav-link">Mentions légales</RouterLink>
          </li>
          <li>
            <RouterLink to="APropos" class="nav-link">À propos de nous</RouterLink>
          </li>
        </ul>
      </nav>
    </div>
  </footer>
</template>

<style scoped>
.color-container {
  background-color: hsl(232 29% 44%);
  color: #EFEFEF;
  padding: 1rem 0; /* padding correct */
  border-radius: 8px;

  /* Centrage horizontal ET vertical */
  display: flex;
  justify-content: center;
  align-items: center;
}

/* La clé pour rester sur une seule ligne */
.footer-links {
  display: flex;             /* flex horizontal */
  justify-content: center;   /* centre horizontalement */
  gap: 2rem;                 /* espace entre les liens */
  list-style: none;          /* supprime les puces */
  margin: 0;
  padding: 0;
  flex-wrap: nowrap;         /* ✅ empêche les liens de passer à la ligne */
}

/* Style des liens */
.nav-link {
  color: #EFEFEF;
  text-decoration: none;
  transition: color 0.3s;
}

.nav-link:hover {
  text-decoration: underline;
  color: hsl(232 40% 80%);
}
</style>
