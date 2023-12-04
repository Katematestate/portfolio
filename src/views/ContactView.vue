<script setup>
import CV from '@/assets/logo.svg';
</script>

<template>
  <section class="grid-2">
    <div class="column">
        <img :src="CV" height="100" width="100" />
        <h1>Cheers!</h1>
        <p>blah blah blah</p>
    </div>
  
    <div class="column">
      <h1>Contact</h1>
      <span>Name:</span>
      <span>Email</span>
      <span>Instagram</span>
      <span>LinkedIn</span>
    </div>

  </section>
</template>