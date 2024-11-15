<template>
  <!-- Contenedor principal para pantallas pequeñas y grandes -->
  <div class="flex flex-col items-center mt-10 space-y-4">
    <!-- Proyectos: Siempre ocupa el 100% del ancho en pantallas pequeñas y centra el contenido en pantallas grandes -->
    <div class="w-full sm:w-auto flex justify-center">
      <MyProyects />
    </div>

    <!-- Contenedor para MySkills y TrainingsCert: En pantallas grandes (sm) los coloca en fila, en pequeñas en columna -->
    <div class="flex flex-col sm:flex-row w-full sm:justify-center sm:space-x-8 space-y-4 sm:space-y-0">
      <div class="flex justify-center w-full sm:w-auto">
        <MySkills />
      </div>
      <div class="flex justify-center w-full sm:w-auto">
        <TrainingsCert />
      </div>
    </div>
  </div>
</template>

<script setup>
import MyProyects from '../components/experience/MyProyects.vue'
import MySkills from '../components/experience/MySkills.vue'
import TrainingsCert from '../components/experience/TrainingsCert.vue'
</script>
