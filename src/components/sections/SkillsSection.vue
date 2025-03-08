<script setup lang="ts">
import { technologies } from '../../data/skills';
import SectionHeader from '../common/SectionHeader.vue';
import { ref } from 'vue';

// Track the currently hovered technology
const hoveredTech = ref<string | null>(null);

const setHoveredTech = (techName: string | null) => {
  hoveredTech.value = techName;
};
</script>

<template>
  <section id="skills" class="py-16 bg-gray-50">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <SectionHeader 
        title="My Skills" 
        subtitle="Technical expertise and proficiencies" 
      />
      
      <div class="w-full">
        <!-- Technologies -->
        <div class="bg-white p-8 rounded-xl shadow-md">
          <h3 class="text-xl font-bold text-primary mb-6">Technologies</h3>
          <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-5 xl:grid-cols-6 gap-6">
            <div 
              v-for="tech in technologies" 
              :key="tech.name" 
              class="flex flex-col items-center relative"
              @mouseenter="setHoveredTech(tech.name)"
              @mouseleave="setHoveredTech(null)"
            >
              <div class="w-16 h-16 rounded-full bg-gray-100 flex items-center justify-center mb-3">
                <i :class="[tech.icon, tech.color, 'text-3xl']"></i>
              </div>
              <span class="text-sm font-medium">{{ tech.name }}</span>
              
              <!-- Sub-technologies popup -->
              <div 
                v-if="hoveredTech === tech.name && tech.subTechnologies?.length" 
                class="absolute top-full mt-2 bg-white shadow-lg rounded-lg p-3 z-10 w-48 transition-opacity duration-200"
              >
                <h4 class="font-bold text-sm mb-2 text-primary">Related Skills:</h4>
                <ul class="space-y-1">
                  <li 
                    v-for="subTech in tech.subTechnologies" 
                    :key="subTech" 
                    class="text-sm text-gray-700"
                  >
                    {{ subTech }}
                  </li>
                </ul>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
/* Add some styles to handle the position and appearance of the popup */
.relative {
  position: relative;
}

.absolute {
  position: absolute;
}

/* Fade animation for popup */
.transition-opacity {
  transition: opacity 0.2s ease-in-out;
}
</style>
