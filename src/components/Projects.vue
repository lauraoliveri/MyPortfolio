<script>

import projectsData from '../data/projects.json';

export default {
  data() {
    return { 
      projects: projectsData
    }
  }
}
</script>

<template>
  <section id="projects">
    <div class="container">
     <div class="row">

      <h1 class="py-5">
        PROJECTS
      </h1>
        <!-- Progetto 1 -->
        <div class="col-md-4 col-12 mb-4"
        v-for="project in projects" 
        :key="index">
          <div class="card p-2">
            <div class="img_square">
              <img :src="project.immagine" :alt="project.nome">
            </div>
            <div>
              <h4>{{ project.nome }}</h4>
              <p>{{ project.descrizione }}</p>
              <a :href="project.link" target="_blank">Visita progetto</a>
            </div>
          </div>
        </div>


      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

section {
  background-image: url(../assets/images/pattern.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  width: 100%;
  height: 700px;
  text-align: center;

  @include underline-on-hover;
}

h1, h4 {
  font-family: 'VT323', sans-serif;
  color: $pink;
}

.card {
  background-color: $white;
  width: 400px;
  text-align: center;
}

.img {
  width: 300px;
  height: 300px;
  text-align: center;
  padding: 10px;
}

a {
  text-decoration: none;
  color: $pink;  

  &:hover{
    color: $black;
  }
}
</style>
