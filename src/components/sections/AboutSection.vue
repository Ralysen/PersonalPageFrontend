<template>
  <section id="about" class="py-16 bg-white">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <SectionHeader 
        title="About Me" 
        subtitle="Who I am and what I do" 
      />
      
      <div class="grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
        <div class="relative">
          <div class="bg-white p-2 rounded-xl shadow-lg">
            <div class="aspect-square rounded-lg overflow-hidden">
              <img src="../../images/zdjecie_about_me.jpg" alt="About me" class="w-full h-full object-cover" />
            </div>
          </div>
          <div class="absolute -z-10 -bottom-4 -right-4 w-48 h-48 bg-green-100 rounded-full opacity-70"></div>
        </div>
        
        <div>
          <h3 class="text-2xl font-bold text-primary mb-4">Backend Developer</h3>
          <p class= "text-gray-600 mb-6">
            I am a junior backend developer with 1+ years of experience. I am strongly related to the Node.js ecosystem and I am proficient in TypeScript, Node.js, Express.js/Nest.js, and PostgreSQL. I am also familiar with other technologies such as Docker, Redis, and AWS.
          </p>
          <p class="text-gray-600 mb-6">
            I'm constantly expanding my knowledge of new technologies and methodologies to ensure I'm delivering the best possible solutions for the challenges at hand.
          </p>
          <div class="flex gap-4 mb-8">
            <a href="#" class="social-icon text-gray-600 hover:text-accent">
              <i class="fab fa-github text-2xl"></i>
            </a>
            <a href="#" class="social-icon text-gray-600 hover:text-accent">
              <i class="fab fa-linkedin text-2xl"></i>
            </a>
            <a href="#" class="social-icon text-gray-600 hover:text-accent">
              <i class="fab fa-twitter text-2xl"></i>
            </a>
            <a href="#" class="social-icon text-gray-600 hover:text-accent">
              <i class="fab fa-dev text-2xl"></i>
            </a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
import SectionHeader from '../common/SectionHeader.vue';
</script>
