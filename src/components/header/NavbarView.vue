<template>
  <nav class="flex items-center bg-transparent w-full max-w-xs mx-5 py-4 rounded">
    <div class="flex flex-row md:flex-col text-xl font-bold space-x-4 md:space-x-0 md:space-y-4 w-full">
      <router-link v-for="(link, index) in links" :key="index" :to="link.path"
        class="no-underline text-white text-center px-3 py-2 transition-all duration-300 hover:underline" href="#">
        {{ link.name }}
      </router-link>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'NavbarView',
  data() {
    return {
      links: [
        { name: 'Home', path: '/' },
        { name: 'About', path: '/about' },
        { name: 'Experiencia', path: '/experiencia' },
      ]
    }
  }
}
</script>
