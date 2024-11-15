<template>

  <!-- Iconos debajo del bloque de texto y más grandes -->
  <div class="flex justify-center mt-20 space-x-6">
    <i v-for="(icon, index) in icons" :key="index" :class="icon.class" @click="redirectTo(icon.url)"
      class="cursor-pointer transition-transform transform hover:scale-110"></i>
  </div>
</template>

<script setup>
import { ref } from 'vue';

// Array de objetos que contiene la información de los iconos
const icons = ref([
  {
    class: 'fa-brands fa-linkedin text-4xl',
    url: 'https://www.linkedin.com/in/csdelartundo',
  },
  {
    class: 'fa-brands fa-github text-4xl',
    url: 'https://github.com/csdelartundo',
  },
  {
    class: 'fa-brands fa-whatsapp text-4xl',
    url: 'https://wa.me/56949359372',
  },
  {
    class: 'fa-regular fa-envelope text-4xl',
    url: 'mailto:csdelartundo@gmail.com',
  },
]);

// Función para redirigir a la URL
const redirectTo = (url) => {
  window.open(url, '_blank');
};
</script>
