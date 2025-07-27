<script>
/* 
  Per importare ed utilizzare un componente dentro un altro devo SEMPRE seguire questi 3 passi:
  1) Importazione del componente
  2) Dichiarazione del componente
  3) Utilizzo del componente
*/
// 1) Importazione del componente
import Hero from './components/Hero.vue';
import About from './components/About.vue';
import Skills from './components/Skills.vue';
import Projects from './components/Projects.vue';
import Contacts from './components/Contacts.vue';
import Footer from './components/Footer.vue';


export default {
  data() {
    return { 
      
    }
  },
  // 2) Dichiarazione del componente
  components: {
    Hero,
    About,
    Skills,
    Projects,
    Contacts,
    Footer

  },
  methods: {
    
  }
}
</script>

<template>
  <div>
    <!-- 3) Utilizzo del componente -->
    <Hero />
    <About/>
    <Skills />
    <Projects />
    <Contacts />
    <Footer />
    
  </div>
</template>

<style lang="scss">
@use 'assets/scss/main' as *;
// Import all of Bootstrap's CSS
@import "bootstrap/scss/bootstrap";

// Import Font
@font-face {
  font-family: 'Relashionship of Melodrame';
  src: url('src/assets//fonts/Relationship_of_melodrame.ttf') format('truetype');
  font-weight: normal;
  font-style: normal;
}

body {
  font-family: "Manrope", sans-serif !important; 
  font-optical-sizing: auto;
  font-weight: 400;
  font-style: normal;
}
</style>
