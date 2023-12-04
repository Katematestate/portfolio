<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Logo from '@/assets/logo.svg';
</script>

<template>
  <div class="root">
    <header>
      <img :src="Logo" alt="" width="60">
      <span>Katie Pragg</span>
      <button>Contact</button>
    </header>

    <aside>
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/projects">Projects</RouterLink>
        <RouterLink to="/contact">Contact</RouterLink>
      </nav>
    </aside>

    <main>
      <RouterView />
    </main>
  </div>
</template>

<style scoped>
.root {
  display: grid;
  grid-template-columns: 100px 1fr;
  grid-template-rows: 70px 1fr;
}

header {
  grid-column: 2;
  background-color: orange;
}

aside {
  grid-column: 1;
  grid-row: 1/span 2;
  background-color: pink;
}

main {
  background-color: aquamarine;
}
</style>
