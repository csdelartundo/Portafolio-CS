<template>
  <div class="flex flex-col items-center justify-center px-4  md:mt-20 md:flex-row md:space-x-8 w-full">
    <!-- Imagen centrada en la parte superior en pantallas pequeñas, a la izquierda en pantallas grandes -->
    <img class="w-40 h-auto md:mb-24 md:w-1/3 md:max-w-xs mt-8" src="/src/assets/img/profile-pic.png"
      alt="profile picture" />

    <!-- Texto centrado debajo de la imagen en pantallas pequeñas y al lado derecho en pantallas grandes -->
    <div class="text-center max-w-2xl mt-8 mb-8">
      <span class="block font-mono font-bold text-2xl mb-4">¡Hola! 👋 Soy Constanza ✨</span>
      <span class="block font-mono font-light text-lg mb-4">
        Egresada de la academia Desafío Latam como desarrolladora front end. Con más de 5 años
        de experiencia en atención al cliente, gestión de eventos y creación de material técnico, estoy en una
        transición del ámbito veterinario al mundo TI. Actualmente, desarrollo
        aplicaciones web, enfocándome en entender las necesidades de los usuarios y ofrecer soluciones efectivas que
        mejoren su experiencia.
      </span>
      <span class="block font-mono font-light text-lg">
        Mi experiencia en el rubro agropecuario, sumada a las habilidades adquiridas en el ámbito TI, me permite aportar
        una visión integral que combina conocimientos técnicos con una gran capacidad para empatizar con los usuarios.
        Me considero una profesional organizada, orientada a resultados y con habilidad para trabajar en equipo. Estoy
        emocionada por contribuir a proyectos que generen un impacto positivo y duradero. ¡Conectemos y exploremos
        nuevas oportunidades para hacer crecer el mundo TI!
      </span>
      <IconsContact />
    </div>
    <!-- <div class="flex flex-row justify-center md:mt-8 space-x-6">
      <IconsContact />
    </div> -->
  </div>

  <!-- Iconos debajo del bloque de texto -->

</template>

<script setup>
import IconsContact from './IconsContact.vue'
</script>
