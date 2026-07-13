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
    <!-- Divider -->
    <hr class="divider mb-5"></hr>

    <div class="container">
      <div class="row">

        <!-- Title -->
        <div class="d-flex align-items-center justify-content-center">
          <h1 class="py-5 fw-bold">
            Projects
          </h1>
        </div>

        <!-- Projects -->
        <div class="col-md-4 col-12 mb-4 d-flex flex-column align-items-center" v-for="project in projects"
          :key="index">
          <div class="card p-2">

            <!-- Image -->
            <div class="img_square">
              <img :src="project.image" :alt="project.name">
            </div>
            <div class="p-2">
              <!-- Name -->
              <h4 class="text-start">
                {{ project.name }}
              </h4>

              <!-- Description -->
              <p class="text-start">{{ project.description }}</p>
            </div>
          </div>

          <!-- Link to project -->
          <!-- <div class="text-start">
            <a :href="project.link">
              <button type="button" class="btn btn-outline text-uppercase">SEE PROJECT</button>
            </a>
          </div> -->
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

section {
  width: 100%;
  min-height: 70vh;
  text-align: center;
}

h1 {
  // Title
  color: white;
}

h4 {
  // Projects names
  font-family: 'VT323', sans-serif;
  color: $pink;
  text-transform: uppercase;
}

.card {
  width: 300px;
  height: 350px;
  margin: 15px;
  border-radius: 15px;

  // Glass Effect
  background: rgba(255, 255, 255, 0.04) !important;
  backdrop-filter: blur(20px) saturate(160%);
  -webkit-backdrop-filter: blur(20px) saturate(160%);

  // Border and neon glow 
  border: 1px solid rgba(255, 255, 255, 0.1);
  box-shadow: 0 15px 35px rgba(0, 0, 0, 0.4);
  transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);

  &:hover {
    // Hover animation
    transform: translateY(-10px);
    box-shadow: 0 0 25px rgba(253, 126, 152, 0.2);
    background: rgba(255, 255, 255, 0.07) !important; 
  }

}

.img_square {

  img {
    min-height: 200px;
    width: 100%;
    border-radius: 10px;
    // Subtle glow for image inside 
    filter: drop-shadow(0 0 10px rgba(253, 126, 152, 0.3));
  }
}

p {
  // Projects description
  color: $white;
}

a {
  text-decoration: none;
  color: $pink;
  // Neon shadow 
  text-shadow:
    0 0 8px rgba($pink, 0.6),
    0 0 16px rgba($pink, 0.4),
    0 0 24px rgba($white, 0.15);

  &:hover {
    color: $deepPurple;
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

// Divider
.divider {
  width: 50%;          
  height: 1px;      
  margin: 0 auto;      
  background: linear-gradient(
    to right, 
    transparent, 
    $pink,            
    transparent
  );
  box-shadow: 0 0 10px rgba(253, 126, 152, 0.4);
  opacity: 0.6;
  border: none;
}
</style>
