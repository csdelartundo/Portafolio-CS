<template>
  <div class="md:flex">
    <header
      class="flex flex-col bg-gradient-to-r from-indigo-500 via-purple-500 to-pink-500 md:flex-row items-center justify-evenly md:h-screen w-full  bg-center sm:bg-cover">

      <!-- Contenido (Navbar y DarkMode) -->
      <div class="flex flex-col items-center md:flex-col md:items-center w-full md:w-auto z-10">
        <NavbarView />
        <!-- Mostrar DarkMode solo en pantallas grandes -->
        <div class="hidden md:block mt-4">
          <DarkMode />
        </div>
      </div>
    </header>
  </div>
</template>
<script setup>
import NavbarView from './NavbarView.vue';
import DarkMode from './DarkMode.vue';
</script>
