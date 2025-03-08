<template>
  <section class="bg-gradient-to-b from-white to-gray-100 py-16 sm:py-24">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
        <div>
          <h1 class="text-4xl sm:text-5xl font-bold text-primary mb-4">
            Hi, I'm <span class="text-accent">Radosław Łysoń</span>
          </h1>
          <h2 class="text-2xl sm:text-3xl font-semibold text-secondary mb-6">
            Backend Developer
          </h2>
          <p class="text-lg text-gray-600 mb-8">
            I build robust, scalable backend solutions and APIs that power modern web applications.
          </p>
          <div class="flex flex-wrap gap-4">
            <a href="#contact" class="btn btn-primary">
              <i class="fas fa-envelope mr-2"></i>Get in touch
            </a>
            <a href="#projects" class="btn border border-gray-300 hover:border-accent hover:text-accent">
              <i class="fas fa-code mr-2"></i>View my work
            </a>
          </div>
        </div>
        <div class="relative">
          <div class="bg-white p-2 rounded-xl shadow-xl">
            <div class="bg-gray-100 rounded-lg aspect-square flex items-center justify-center overflow-hidden">
              <img src="../../images/zdjęcie CV.jpg" alt="Radosław Łysoń" class="w-full h-full object-cover" />
            </div>
          </div>
          <!-- Decorative element -->
          <div class="absolute -z-10 -bottom-6 -right-6 w-64 h-64 bg-blue-100 rounded-full opacity-70"></div>
          <div class="absolute -z-10 -top-6 -left-6 w-48 h-48 bg-yellow-100 rounded-full opacity-70"></div>
        </div>
      </div>
    </div>
  </section>
</template>
