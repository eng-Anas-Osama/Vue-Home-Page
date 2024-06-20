<template>
    <header>
        <div class="container mx-auto flex items-center justify-between p-4">
      <!-- Logo -->
      <div class="text-2xl font-bold">
        <a href="#"><img src="{{ logo }}"></a>
      </div>

      <!-- Menu (hidden on small screens) -->
      <nav class="hidden md:flex space-x-4">
        <a href="#" class="text-gray-700 hover:text-blue-500">Home</a>
        <a href="#" class="text-gray-700 hover:text-blue-500">About</a>
        <a href="#" class="text-gray-700 hover:text-blue-500">Services</a>
        <a href="#" class="text-gray-700 hover:text-blue-500">Contact</a>
      </nav>

      <!-- Call to Action Button -->
      <div class="hidden md:block">
        <button class="btn btn-primary">Get Started</button>
      </div>

      <!-- Mobile menu button -->
      <div class="md:hidden">
        <button @click="toggleMenu" class="text-gray-700 focus:outline-none">
          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" class="w-6 h-6">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
          </svg>
        </button>
      </div>
    </div>

    <!-- Mobile menu (hidden by default) -->
    <div v-if="isMenuOpen" class="md:hidden bg-white border-t border-gray-200">
      <nav class="p-4 space-y-2">
        <a href="#" class="block text-gray-700 hover:text-blue-500">Home</a>
        <a href="#" class="block text-gray-700 hover:text-blue-500">About</a>
        <a href="#" class="block text-gray-700 hover:text-blue-500">Services</a>
        <a href="#" class="block text-gray-700 hover:text-blue-500">Contact</a>
        <button class="btn btn-primary w-full">Get Started</button>
      </nav>
    </div>
    </header>
</template>

<script>
export default {
  data() {
    return {
      isMenuOpen: false,
    }
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    }
  }
}
</script>

<style scoped>
/* Additional styles if needed */
</style>