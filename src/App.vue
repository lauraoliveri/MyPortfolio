<script>

import Hero from './components/Hero.vue';
import About from './components/About.vue';
import Skills from './components/Skills.vue';
import Projects from './components/Projects.vue';
import Footer from './components/Footer.vue';
import Contacts from './components/Contacts.vue';


export default {
  data() {
    return { 
      
    }
  },
  components: {
    Hero,
    About,
    Skills,
    Projects,
    Footer,
    Contacts

  },
  methods: {
    
  }
}
</script>

<template>
  <div>
    <Hero/>
    <About/>
    <Contacts/>
    <Skills/>
    <Projects/>
    <Footer/>
    
  </div>
</template>

<style lang="scss">
@use 'assets/scss/main' as *;
// Import all of Bootstrap's CSS
@import "bootstrap/scss/bootstrap";

// Import Font
@font-face {
  font-family: 'UncutSans';
  src: url('src/assets//fonts/UncutSans-Variable.ttf') format('truetype');
  font-weight: 100 900;
  font-style: normal;
}

// Set Font
body {
  font-family: "UncutSans", sans-serif !important;
  font-weight: 500; 
}


*::selection {
  background-color: $pink;
}
</style>
