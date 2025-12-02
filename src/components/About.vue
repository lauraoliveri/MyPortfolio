<script>
export default {
  data() {
    return {

    }
  }
}
</script>

<template>
  <section id="about">
    <div class="container about_me py-5">
      <div class="row">

        <!-- left part: description -->
        <div class="col-md-6 col-12">
          <div class="d-flex align-items-center">
            <div class="pe-2 ">
              <img src="/src/assets/images/flower.svg" alt="">
            </div>
            <h1 class="text-uppercase">
              ⎯ ABOUT ME
            </h1>
          </div>

          <!-- paragraph about me -->
          <p class=" pb-2">
            I’m a 22-year-old, curious and determined aspiring developer, always ready to learn and grow.<br><br>
            After fulfilling my childhood dream of working as a flight attendant, I discovered a new passion: computer
            science.<br>
            This led me to complete an intensive 700-hour course in <strong>front-end</strong> and
            <strong>back-end</strong> development,
            where I gained solid skills and a strong desire to keep learning. I also completed a course in Java, further
            expanding my programming skillset.<br><br>
            <span class="text-decoration-underline">I’m now looking for my first professional opportunity in IT</span>,
            excited to apply my skills, contribute to real projects, and continue growing as a web developer.<br>
            In my free time, I enjoy music, playing guitar, reading, gaming… and watching too many adorable cat videos
            online!:) <br><br>
          </p>

          <!-- resume button -->
          <div>
            <button type="button" class="btn btn-outline text-uppercase">View Resume</button>
          </div>
        </div>

        <!-- right part with pic -->
        <div class="col-md-6 col-12 text-end">
          <img src="/src/assets/images/me.png" alt="" class="polaroid">
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
  min-height: 90vh;
}


.polaroid {
  width: 335px;
  padding-top: 20px;
  transform: rotate(5deg);
}

.about_me {
  h1 {
    color: $pink;
    text-decoration: none;
    font-family: 'VT323', sans-serif;
  }

  p {
    font-size: large;
  }

}

// Button

.btn-outline {
  font-size: larger;
  font-family: $btn-font-family;
  font-weight: $btn-font-weight;
  color: $btn-outline-color;
  background-color: $btn-outline-bg;
  border: 2px solid $btn-outline-border;
  border-radius: $btn-outline-border-radius;

  /* Neon shadow */
  box-shadow:
    0 0 8px rgba($pink, 0.6),
    0 0 16px rgba($pink, 0.4),
    0 0 24px rgba($white, 0.15);

  &:hover {
    background-color: $btn-outline-hover-bg;
    color: $btn-outline-hover-color;
    border-color: $btn-outline-hover-border;

  }

}
</style>
