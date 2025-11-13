<script>

import skillsData from '../data/skills.json';

export default {
  data() {
    return { 
      skills: skillsData.skills,
      currentlyLearning: skillsData.currentlyLearning
    }
  }
}
</script>

<template>
  <section id="skills" class="py-5">
    <div class="container">
      <h1 class="text-center mb-5">SKILLS</h1>

      <!-- Skills -->
      <div class="d-flex flex-wrap justify-content-center gap-4">
        <div
          v-for="skill in skills"
          :key="skill.name"
          class="d-flex flex-column align-items-center skill_item"
          style="flex: 1 1 calc(20% - 1rem);" 
        >
          <img :src="skill.image" :alt="skill.name" class="skill_img mb-2"/>
          <p class="text-uppercase text-center">{{ skill.name }}</p>
        </div>
      </div>

      <!-- Learning -->
      <h3 class="text-center text-uppercase mt-5 mb-4">
        Currently Learning:
      </h3>

      <div class="d-flex flex-wrap justify-content-center gap-4">
        <div
          v-for="skill in currentlyLearning"
          :key="skill.name"
          class="d-flex flex-column align-items-center skill_item"
          style="flex: 1 1 calc(20% - 1rem);"
        >
          <img :src="skill.image" :alt="skill.name" class="skill_img mb-2"/>
          <p class="text-uppercase text-center">{{ skill.name }}</p>
        </div>
      </div>
    </div>
  </section>
</template>



<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;


section {
  background-color: $black;
  color: $white;
  width: 100%;
  min-height: 100vh;
  text-align: center;

  @include underline-on-hover;
}

h1, h3{
  font-family: 'VT323', sans-serif;  
  color: $pink;
}

.items_contaneir {
  padding-left: 300px;
  padding-right: 300px;
}

.skill_item {
  padding-right: 30px;
  padding-bottom: 30px;
}

.skill_img {
  width: 100px;
  padding-bottom: 10px;
}
</style>
