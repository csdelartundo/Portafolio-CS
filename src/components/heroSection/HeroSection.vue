<template>
  <div class="flex justify-center items-center w-full px-4 py-10 mt-10">
    <!-- Eliminar h-screen, agregar py-10 para espaciado -->
    <div class="flex flex-col md:flex-row w-full items-center justify-center space-y-6 md:space-y-0 md:space-x-10">
      <!-- Añadir espacio entre los elementos -->
      <!-- Contenedor de textos alineados a la izquierda -->
      <div class="flex flex-col md:w-2/3 space-y-4 items-center font-mono">
        <span class="text-5xl font-bold text-center">Constanza Salinas de Lartundo</span>
        <span class="text-4xl font-semibold text-center md:text-left">Desarrolladora Front End</span>
      </div>

      <!-- Imagen alineada a la derecha -->
      <div class="w-full md:w-1/3 flex justify-center pt-5">
        <SvgIcon class="w-full h-auto max-w-xs" />
      </div>
    </div>
  </div>

  <!-- Contenedor para los íconos de contacto centrados debajo del texto y la imagen -->
  <div class="flex justify-center mb-6">
    <IconsContact />
  </div>
</template>

<script setup>
import SvgIcon from "./SvgIcon.vue";
import IconsContact from "../about/IconsContact.vue";
</script>
