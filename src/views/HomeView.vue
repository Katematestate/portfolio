<script setup>
import Portrait from '@/assets/logo.svg';
import Carousel from 'primevue/carousel';
const projects = [
  {
    name: 'cactus', image: Portrait, link: '/projects/1'
  },
  {
    name: 'zombie', image: Portrait, link: '/projects/2'
  },
  {
    name: 'shire', image: Portrait, link: '/projects/3'
  },
  {
    name: 'cactus', image: Portrait, link: '/projects/1'
  },
  {
    name: 'zombie', image: Portrait, link: '/projects/2'
  },
  {
    name: 'shire', image: Portrait, link: '/projects/3'
  },

]
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
      <Carousel :value="projects" :numVisible="3" :numScroll="3">
        <template #item="slotProps">
          <div class="project-container">
            <img :src="slotProps.data.image" :title="slotProps.data.name" :alt="slotProps.data.name" />
            <span>{{ slotProps.data.name }}</span>
            <button>View</button>
          </div>
        </template>
      </Carousel>
      <h2>Work</h2>
      <div class="carousel">
        <img :src="Portrait" alt="" width="80">
        <img :src="Portrait" alt="" width="80">
        <img :src="Portrait" alt="" width="80">
      </div>
      <h2>Personal</h2>
      <div class="carousel">
        <img :src="Portrait" alt="" width="80">
        <img :src="Portrait" alt="" width="80">
        <img :src="Portrait" alt="" width="80">
      </div>
    </section>
  </div>
</template>

<style scoped>
.project-container{
  display: flex;
  flex-direction: column;
  gap: 8px;
  padding: 16px;
  margin: 0 8px;
  border: 2px solid #003463;
  border-radius: 8px;
  background-color: blanchedalmond;
  width: auto;
}

h2{
  text-align: center;
}

</style>

