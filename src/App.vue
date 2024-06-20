<script setup>
import Header from './components/Header.vue';
import HelloWorld from './components/HelloWorld.vue'
import NaveBar from './components/NaveBar.vue'
import './index.css'; 
</script>


<template>
  <Header logo="https://thumbs.dreamstime.com/z/lets-shopping-logo-design-template-cart-icon-designs-134743663.jpg" />
  <div class="min-h-screen bg-gray-100 p-4">
      <header class="text-center mb-6">
        <h1 class="text-4xl font-bold mb-2">My Vue App with Tailwind CSS and DaisyUI</h1>
        <p class="text-lg text-gray-600">Building awesome web pages!</p>
      </header>
  </div>
  
  

</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
