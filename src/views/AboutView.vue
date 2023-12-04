<script setup>
import CV from '@/assets/logo.svg';
</script>

<template>
  <section class="grid-2">
    <div class="about">
      <h1>This is an about page</h1>
      <div class="para-img-flip">
        <img :src="CV" height="100" width="100" />
        <p>blah blah blah</p>
      </div>
      <div class="para-img-flip">
        <img :src="CV" height="100" width="100" />
        <p>blah blah blah</p>
      </div>
      <div class="para-img-flip">
        <img :src="CV" height="100" width="100" />
        <p>blah blah blah</p>
      </div>
      <div class="para-img-flip">
        <img :src="CV" height="100" width="100" />
        <p>blah blah blah</p>
      </div>
    </div>
  
    <div class="cv">
      <h1>CV</h1>
      <img :src="CV" height="150" width="150" />
    </div>
  </section>
</template>


