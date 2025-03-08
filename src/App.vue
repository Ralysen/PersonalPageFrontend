<script setup lang="ts">
import Navbar from './components/layout/Navbar.vue';
import Footer from './components/layout/Footer.vue';
import HeroSection from './components/sections/HeroSection.vue';
import AboutSection from './components/sections/AboutSection.vue';
import SkillsSection from './components/sections/SkillsSection.vue';
// import ProjectsSection from './components/sections/ProjectsSection.vue';
// import BlogSection from './components/sections/BlogSection.vue';
import ContactSection from './components/sections/ContactSection.vue';
</script>

<template>
  <div class="bg-gray-50 text-gray-800">
    <Navbar />
    <HeroSection />
    <AboutSection />
    <SkillsSection />
    <!-- <ProjectsSection /> -->
    <!-- <BlogSection /> -->
    <ContactSection />
    <Footer />
  </div>
</template>

<style>
@import './assets/styles/main.css';
</style>