<script setup>
import NavbarVue from './components/Navbar.vue'
import ContentVue from './components/Content.vue'
</script>

<template>
  <header>
    <NavbarVue/>
  </header>
  <main>
    <ContentVue/>
  </main>
  <footer class="attribution text-center my-5" style="width:21rem ;margin: auto;">
      Challenge by <a href="https://www.frontendmentor.io/challenges/intro-section-with-dropdown-navigation-ryaPetHE5" target="_blank">Frontend Mentor</a>. 
      Coded by <a href="https://www.linkedin.com/in/salahudheen-k-7574ba1a6/" target="_blank">Salahudheen</a>.
    </footer>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
