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

        <!-- Title -->
        <div class="d-flex align-items-center justify-content-center">
          <div class="pe-2 ">
            <img src="/src/assets/images/flower.svg" alt="">
          </div>
          <h1 class="py-5 text-uppercase">
            ⎯ PROJECTS
          </h1>
        </div>

        <!-- Projects -->
        <div class="col-md-4 col-12 mb-4" v-for="project in projects" :key="index">
          <div class="card p-2">
            <div class="img_square">
              <img :src="project.immagine" :alt="project.nome">
            </div>
            <div class="p-2">
              <h3><a :href="project.link" target="_blank">
                  {{ project.nome }}
                </a></h3>
              <p class="text-start">{{ project.descrizione }}</p>

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

  width: 100%;
  height: 700px;
  text-align: center;

}

h1,
h3 {
  font-family: 'VT323', sans-serif;
  color: $pink;
}

.card {
  height: 400px;
  background-color: #1d131320;
  width: 400px;
  text-align: center;
}

.img_square {

  text-align: center;
  padding: 10px;

  img {
    min-height: 200px;
    width: 100%;
    border-radius: 5px;
  }
}

p {
  color: $white;
}

a {
  text-decoration: none;
  color: $pink;
  /* Neon shadow */
  text-shadow:
    0 0 8px rgba($pink, 0.6),
    0 0 16px rgba($pink, 0.4),
    0 0 24px rgba($white, 0.15);

  &:hover {
    color: $black;
  }
}
</style>
