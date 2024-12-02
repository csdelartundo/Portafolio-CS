<template>
  <div class="flex flex-col items-center space-y-4 p-6 bg-gray-100 rounded-lg shadow-md mx-4">
    <!-- Título de la sección -->
    <span class="text-3xl font-bold font-mono text-center text-blue-600 mb-6">Proyectos</span>

    <!-- Contenedor para proyectos -->
    <div class="flex flex-col sm:flex-row sm:space-x-8 space-y-8 sm:space-y-0">
      <!-- Primer proyecto -->
      <div
        class="flex flex-col items-center space-y-2 bg-blue-100 rounded-md p-3 shadow-sm hover:bg-blue-200 transition-colors">
        <div class="group relative">
          <img src="/src/assets/img/pokeapp.png" alt="Pokemon App"
            class="w-48 mb-6 h-auto transition-transform transform group-hover:scale-105" />
        </div>
        <a href="https://prueba-interfaz-interactiva-vue-js-pokemon.vercel.app/" target="_blank" class="text-blue-800 ">
          Pokemon App
        </a>
      </div>

      <!-- Segundo proyecto -->
      <div
        class="flex flex-col items-center space-y-2 bg-blue-100 rounded-md p-3 shadow-sm hover:bg-blue-200 transition-colors">
        <div class="group relative">
          <img src="/src/assets/img/elchilenoweb.png" alt="Web El Chileno"
            class="w-48 h-auto transition-transform transform group-hover:scale-105" />
        </div>
        <a href="https://elchileno.vercel.app/" target="_blank"
          class="bg-blue-100 text-blue-800 rounded-md p-3 shadow-sm hover:bg-blue-200 transition-colors">
          Pyme "El Chileno Temático"
        </a>
      </div>

      <!-- Tercer proyecto -->
      <div
        class="flex flex-col items-center space-y-2 bg-blue-100 rounded-md p-3 shadow-sm hover:bg-blue-200 transition-colors">
        <div class="group relative">
          <img src="/src/assets/img/todolist.png" alt="To Do List"
            class="w-48 h-auto transition-transform transform group-hover:scale-105" />
        </div>
        <a href="https://elchileno.vercel.app/" target="_blank"
          class="bg-blue-100 text-blue-800 rounded-md p-3 shadow-sm hover:bg-blue-200 transition-colors">
          To Do List
        </a>
      </div>
    </div>
  </div>
</template>
