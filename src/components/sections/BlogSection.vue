<script setup lang="ts">
import { blogPosts } from '../../data/blogPosts';
import SectionHeader from '../common/SectionHeader.vue';
</script>

<template>
  <section id="blog" class="py-16 bg-gray-50">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <SectionHeader 
        title="Blog" 
        subtitle="Insights and articles about backend development" 
      />
  
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
        <div v-for="post in blogPosts" :key="post.title" class="bg-white rounded-xl shadow-md overflow-hidden transition-transform hover:-translate-y-2">
          <div class="h-48 overflow-hidden">
            <img :src="post.image" :alt="post.title" class="w-full h-full object-cover" />
          </div>
          <div class="p-6">
            <div class="text-sm text-gray-500 mb-2">{{ post.date }}</div>
            <h3 class="text-xl font-bold text-primary mb-2">{{ post.title }}</h3>
            <p class="text-gray-600 mb-4">{{ post.excerpt }}</p>
            <a href="#" class="text-accent hover:underline inline-flex items-center">
              Read More <i class="fas fa-arrow-right ml-1"></i>
            </a>
          </div>
        </div>
      </div>
  
      <div class="text-center mt-10">
        <a href="#" class="btn btn-primary">
          <i class="fas fa-book-open mr-2"></i>View All Articles
        </a>
      </div>
    </div>
  </section>
</template>
