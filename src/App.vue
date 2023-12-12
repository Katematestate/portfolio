<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Logo from '@/assets/katetextlogo.svg';
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Young+Serif&display=swap');
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;600;700;800;900&display=swap');
</style>

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
  background: linear-gradient(to right, #fcf4a3, #ffc30b);
}

aside {
  grid-column: 1;
  grid-row: 1/span 2;
  background: linear-gradient(#fcf4a3, #ffc30b);
}

main {
  background: #fafafa;
}

</style>
