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
  <section id="skills">
    <h2 class="py-5">
      SKILLS
    </h2>

    <!-- Icons container -->
    <div class="items_contaneir">
      <div class="d-flex flex-wrap">
        <div v-for="skill in skills" :key="skill.name" class="col-3 skill_item" >
          <img :src="skill.image" :alt="skill.name" class="skill_img"/>
          <p class="text-uppercase">{{ skill.name }}</p>
        </div>
      </div>

      <!-- Learning -->
      <h3 class="text-uppercase pb-5 pt-2">
        Currently Learning:
      </h3>

      <div class="d-flex flex-wrap pb-5"> 
        <div v-for="skill in currentlyLearning" :key="skill.name" class="col skill_item">
          <img :src="skill.image" :alt="skill.name" class="skill_img"/>
          <p class="text-uppercase">{{ skill.name }}</p>
        </div>
      </div>
    </div>
    <hr class="my-0 pb-4" />
  </section>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;


section {
  background-color: $custom_white;
  text-align: center;
}

h2, h3{
  font-family: 'VT323', sans-serif;  
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
