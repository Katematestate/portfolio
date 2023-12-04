<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Logo from '@/assets/katelogo.svg';
</script>

<template>
  <div class="root">
    <header>
      <img :src="Logo" alt="" width="100">
        <button>Contact</button>
    </header>

    <aside>
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/projects">Projects</RouterLink>
        <RouterLink to="/contact">Contact</RouterLink>
      </nav>

      <div class="social-media">

      </div>
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
  grid-template-rows: auto 1fr;
}

header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 16px;
  background-color: #fcf4a3;
}

aside {
  grid-column: 1;
  grid-row: 1/span 2;
  background-color: #ffc30b;
}

main {
  background-color: #fafafa;
}
</style>
