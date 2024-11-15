<template>
  <div class="flex flex-col items-center space-y-2 p-6 bg-gray-100 rounded-md shadow-md ml-5 max-w-3xl">
    <span class="text-3xl font-bold font-mono text-center text-blue-600 mb-6">Skills</span>

    <!-- Contenedor de habilidades con disposición horizontal en pantallas grandes -->
    <div class="flex flex-col sm:flex-row flex-wrap gap-4 justify-center text-center">
      <!-- Contenedor para la primera fila de habilidades -->
      <div class="flex flex-wrap gap-4 justify-center w-full">
        <!-- Iteración de las primeras 5 habilidades -->
        <div v-for="(skill, index) in skills.slice(0, 5)" :key="index"
          class="flex items-center space-x-2  justify-center  bg-blue-100 rounded-md p-3 shadow-sm hover:bg-blue-200 transition-colors">
          <component :is="skill.component || 'i'" :class="`${skill.icon} text-3xl`" :style="{ color: skill.color }" />
          <span class="font-medium text-lg text-blue-800">{{
            skill.name }}</span>
        </div>
      </div>

      <!-- Contenedor para la segunda fila de habilidades -->
      <div class="flex flex-wrap gap-4 justify-center w-full">
        <!-- Iteración de las siguientes 5 habilidades -->
        <div v-for="(skill, index) in skills.slice(5, 10)" :key="index"
          class="flex items-center space-x-2 justify-center bg-blue-100 rounded-md p-3 shadow-sm hover:bg-blue-200 transition-colors">
          <component :is="skill.component || 'i'" :class="`${skill.icon} text-3xl`" :style="{ color: skill.color }" />
          <span class="font-medium text-lg text-blue-800">
            {{ skill.name }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import SvgFirebase from './SVG/SvgFirebase.vue'
import SvgJest from './SVG/SvgJest.vue'
import SvgTailwind from './SVG/SvgTailwind.vue'

export default {
  components: {
    SvgJest,
    SvgFirebase,
    SvgTailwind,
  },
  setup() {
    // Definición de habilidades con icono, color y nombre
    const skills = [
      { name: "HTML", icon: "fa-brands fa-html5", color: "#ff571f" },
      { name: "CSS", icon: "fa-brands fa-css3-alt", color: "#74C0FC" },
      { name: "Sass", icon: "fa-brands fa-sass", color: "#f52eac" },
      { name: "Bootstrap", icon: "fa-brands fa-bootstrap", color: "#670495" },
      { name: "Tailwind", component: "SvgTailwind" },
      { name: "Git", icon: "fa-brands fa-git-alt", color: "#ff571f" },
      { name: "JavaScript", icon: "fa-brands fa-square-js", color: "#FFD43B" },
      { name: "Vue", icon: "fa-brands fa-vuejs", color: "#24ff6d" },
      { name: "Jest", component: "SvgJest" },
      { name: "Firebase", component: "SvgFirebase" },
    ];

    return { skills };
  },
};
</script>
