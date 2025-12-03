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
        <div class="col-md-4 col-12 mb-4 d-flex flex-column align-items-center" v-for="project in projects" :key="index">
          <div class="card p-2">

            <!-- Image -->
            <div class="img_square">
              <img :src="project.image" :alt="project.name">
            </div>
            <div class="p-2">
              <!-- Name -->
              <h3>
                {{ project.name }}
              </h3>

              <!-- Description -->
              <p class="text-start">{{ project.description }}</p>
            </div>
          </div>

          <!-- Link to project -->
          <div class="text-start">
            <a :href="project.link">
              <button type="button" class="btn btn-outline text-uppercase">SEE PROJECT</button>
            </a>
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
  min-height: 90vh;
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
  width: 100%;
  max-width: 400px;
  text-align: center;
  margin: 0 auto; 
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

.btn-outline {
  font-size: large;
  font-family: $btn-font-family;
  font-weight: $btn-font-weight;
  color: $white;


  /* Neon shadow */

  &:hover {
    color: $white;
    text-decoration: underline;

  }

}
</style>
