<script setup lang="ts">
import { projects } from '../../data/projects';
import SectionHeader from '../common/SectionHeader.vue';
</script>

<template>
  <section id="projects" class="py-16 bg-white">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <SectionHeader 
        title="My Projects" 
        subtitle="Recent work and case studies" 
      />
      
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
        <div v-for="project in projects" :key="project.title" class="bg-white rounded-xl shadow-md overflow-hidden transition-transform hover:-translate-y-2">
          <div class="h-48 overflow-hidden">
            <img :src="project.image" :alt="project.title" class="w-full h-full object-cover" />
          </div>
          <div class="p-6">
            <h3 class="text-xl font-bold text-primary mb-2">{{ project.title }}</h3>
            <p class="text-gray-600 mb-4">{{ project.description }}</p>
            <div class="flex flex-wrap gap-2 mb-4">
              <span v-for="tag in project.tags" :key="tag" class="px-3 py-1 bg-gray-100 text-gray-700 rounded-full text-xs">
                {{ tag }}
              </span>
            </div>
            <div class="flex gap-3">
              <a :href="project.github" class="text-gray-600 hover:text-accent">
                <i class="fab fa-github mr-1"></i> Code
              </a>
              <a :href="project.demo" class="text-gray-600 hover:text-accent">
                <i class="fas fa-external-link-alt mr-1"></i> Demo
              </a>
            </div>
          </div>
        </div>
      </div>
  
      <div class="text-center mt-10">
        <a href="#" class="btn btn-primary">
          <i class="fas fa-folder-open mr-2"></i>View All Projects
        </a>
      </div>
    </div>
  </section>
</template>
