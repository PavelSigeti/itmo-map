<template>
  <main>
    <div class="level-image">
      <viewer :options="options" :images="images">
        <div class="img-item">
          <img src="/src/assets/levels/1.jpeg" alt="1">
          <span>1 этаж</span>
        </div>
        <div class="img-item">
          <img src="/src/assets/levels/2.jpeg" alt="2">
          <span>2 этаж</span>
        </div>
        <div class="img-item">
          <img src="/src/assets/levels/3.jpeg" alt="3">
          <span>3 этаж</span>
        </div>
        <div class="img-item">
          <img src="/src/assets/levels/4.jpeg" alt="4">
          <span>4 этаж</span>
        </div>
        <div class="img-item">
          <img src="/src/assets/levels/5.jpeg" alt="5">
          <span>5 этаж</span>
        </div>
      </viewer>
    </div>

    
  </main>
</template>


<script setup>
import {ref} from 'vue';

const current = ref(1);
const images = [
  '/src/assets/levels/1.jpeg',
  '/src/assets/levels/2.jpeg',
  '/src/assets/levels/3.jpeg',
  '/src/assets/levels/4.jpeg',
  '/src/assets/levels/5.jpeg',
];

const options = { 
  'title': false,
  "toolbar": false
};

</script>