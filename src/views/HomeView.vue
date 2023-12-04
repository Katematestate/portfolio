<script setup>
import Portrait from '@/assets/logo.svg';
</script>

<template>
  <div class="grid-2">
    <section>
      <h2>Intro</h2>
      <img :src="Portrait" height="150" width="150" />

      <p>home page blurb</p>
    </section>

    <section>
      <h2>Projects</h2>
      <div class="carousel">
        <img :src="Portrait" alt="" width="80">
        <img :src="Portrait" alt="" width="80">
        <img :src="Portrait" alt="" width="80">
      </div>
      <h2>Projects</h2>
      <div class="carousel">
        <img :src="Portrait" alt="" width="80">
        <img :src="Portrait" alt="" width="80">
        <img :src="Portrait" alt="" width="80">
      </div>
      <h2>Projects</h2>
      <div class="carousel">
        <img :src="Portrait" alt="" width="80">
        <img :src="Portrait" alt="" width="80">
        <img :src="Portrait" alt="" width="80">
      </div>
    </section>
  </div>

</template>

<style scoped>

</style>

