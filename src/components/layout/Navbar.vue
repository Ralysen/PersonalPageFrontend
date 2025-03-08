<script setup lang="ts">
import { ref } from 'vue'

const mobileMenuOpen = ref(false)

const toggleMobileMenu = () => {
  mobileMenuOpen.value = !mobileMenuOpen.value
}
</script>

<template>
  <header class="sticky top-0 z-50 bg-white/90 backdrop-blur-sm shadow-sm">
    <nav class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex justify-between h-16 items-center">
        <div class="flex-shrink-0">
          <a href="#" class="font-bold text-xl text-primary">Radosław<span class="text-accent">Łysoń</span></a>
        </div>
        <div class="hidden md:block">
          <div class="ml-10 flex items-center space-x-8">
            <a href="#about" class="nav-link">About</a>
            <a href="#skills" class="nav-link">Skills</a>
            <a href="#projects" class="nav-link">Projects</a>
            <a href="#blog" class="nav-link">Blog</a>
            <a href="#contact" class="nav-link">Contact</a>
            <a href="#" class="btn btn-primary">Resume</a>
          </div>
        </div>
        <div class="md:hidden">
          <button @click="toggleMobileMenu" class="text-gray-700 hover:text-accent">
            <i class="fas fa-bars text-2xl"></i>
          </button>
        </div>
      </div>
    </nav>
    
    <!-- Mobile menu, show/hide based on menu state -->
    <div v-show="mobileMenuOpen" class="md:hidden">
      <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
        <a href="#about" class="block px-3 py-2 nav-link">About</a>
        <a href="#skills" class="block px-3 py-2 nav-link">Skills</a>
        <a href="#projects" class="block px-3 py-2 nav-link">Projects</a>
        <a href="#blog" class="block px-3 py-2 nav-link">Blog</a>
        <a href="#contact" class="block px-3 py-2 nav-link">Contact</a>
        <a href="#" class="block px-3 py-2 mt-4 btn btn-primary">Resume</a>
      </div>
    </div>
  </header>
</template>
