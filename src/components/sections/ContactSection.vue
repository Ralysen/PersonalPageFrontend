<template>
  <section id="contact" class="py-16 bg-white">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <SectionHeader 
        title="Get In Touch" 
        subtitle="Have a project in mind or want to collaborate? Let's talk!" 
      />
  
      <div class="grid grid-cols-1 md:grid-cols-2 gap-12">
        <div>
          <div class="mb-8">
            <h3 class="text-xl font-bold text-primary mb-4">Contact Information</h3>
            <div class="space-y-4">
              <div class="flex items-start">
                <div class="mr-4 mt-1">
                  <i class="fas fa-envelope text-accent"></i>
                </div>
                <div>
                  <h4 class="font-medium">Email</h4>
                  <p class="text-gray-600">radoslawlyson@gmail.com</p>
                </div>
              </div>
              <div class="flex items-start">
                <div class="mr-4 mt-1">
                  <i class="fas fa-map-marker-alt text-accent"></i>
                </div>
                <div>
                  <h4 class="font-medium">Location</h4>
                  <p class="text-gray-600">Zielona Góra, PL</p>
                </div>
              </div>
              <div class="flex items-start">
                <div class="mr-4 mt-1">
                  <i class="fas fa-clock text-accent"></i>
                </div>
                <div>
                  <h4 class="font-medium">Working Hours</h4>
                  <p class="text-gray-600">Mon - Fri: 8:00 - 16:00</p>
                </div>
              </div>
            </div>
          </div>
      
          <div>
            <h3 class="text-xl font-bold text-primary mb-4">Follow Me</h3>
            <div class="flex gap-4">
              <a href="#" class="w-10 h-10 rounded-full bg-gray-100 hover:bg-accent hover:text-white flex items-center justify-center text-gray-600 transition-colors">
                <i class="fab fa-github"></i>
              </a>
              <a href="#" class="w-10 h-10 rounded-full bg-gray-100 hover:bg-accent hover:text-white flex items-center justify-center text-gray-600 transition-colors">
                <i class="fab fa-linkedin-in"></i>
              </a>
              <a href="#" class="w-10 h-10 rounded-full bg-gray-100 hover:bg-accent hover:text-white flex items-center justify-center text-gray-600 transition-colors">
                <i class="fab fa-twitter"></i>
              </a>
              <a href="#" class="w-10 h-10 rounded-full bg-gray-100 hover:bg-accent hover:text-white flex items-center justify-center text-gray-600 transition-colors">
                <i class="fab fa-dev"></i>
              </a>
            </div>
          </div>
        </div>
  
        <div class="bg-gray-50 p-8 rounded-xl shadow-md">
          <h3 class="text-xl font-bold text-primary mb-6">Send Me a Message</h3>
          <form>
            <div class="mb-4">
              <label for="name" class="block text-sm font-medium text-gray-700 mb-1">Name</label>
              <input type="text" id="name" class="w-full px-4 py-2 border border-gray-300 rounded-md focus:ring-accent focus:border-accent" />
            </div>
            <div class="mb-4">
              <label for="email" class="block text-sm font-medium text-gray-700 mb-1">Email</label>
              <input type="email" id="email" class="w-full px-4 py-2 border border-gray-300 rounded-md focus:ring-accent focus:border-accent" />
            </div>
            <div class="mb-4">
              <label for="subject" class="block text-sm font-medium text-gray-700 mb-1">Subject</label>
              <input type="text" id="subject" class="w-full px-4 py-2 border border-gray-300 rounded-md focus:ring-accent focus:border-accent" />
            </div>
            <div class="mb-6">
              <label for="message" class="block text-sm font-medium text-gray-700 mb-1">Message</label>
              <textarea id="message" rows="4" class="w-full px-4 py-2 border border-gray-300 rounded-md focus:ring-accent focus:border-accent"></textarea>
            </div>
            <button type="submit" class="btn btn-primary w-full">
              <i class="fas fa-paper-plane mr-2"></i>Send Message
            </button>
          </form>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
import SectionHeader from '../common/SectionHeader.vue';
</script>
