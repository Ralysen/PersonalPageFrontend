<template>
  <footer class="bg-gray-800 text-white py-10">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center">
        <a href="#" class="font-bold text-xl mb-4 inline-block">Radosław<span class="text-accent">Łysoń</span></a>
        <div class="flex justify-center gap-6 mb-6">
          <a href="#" class="text-gray-400 hover:text-white">
            <i class="fab fa-github"></i>
          </a>
          <a href="#" class="text-gray-400 hover:text-white">
            <i class="fab fa-linkedin-in"></i>
          </a>
          <a href="#" class="text-gray-400 hover:text-white">
            <i class="fab fa-twitter"></i>
          </a>
          <a href="#" class="text-gray-400 hover:text-white">
            <i class="fab fa-dev"></i>
          </a>
        </div>
        <div class="flex justify-center gap-6 mb-6 text-gray-400">
          <a href="#about" class="hover:text-white">About</a>
          <a href="#skills" class="hover:text-white">Skills</a>
          <a href="#projects" class="hover:text-white">Projects</a>
          <a href="#blog" class="hover:text-white">Blog</a>
          <a href="#contact" class="hover:text-white">Contact</a>
        </div>
        <p class="text-gray-400">© {{ new Date().getFullYear() }} Radosław Łysoń. All rights reserved.</p>
      </div>
    </div>
  </footer>
</template>
