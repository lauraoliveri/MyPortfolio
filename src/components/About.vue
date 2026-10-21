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

        <!-- Title -->
        <div class="col-md-6 col-12">
          <div class="d-flex align-items-center">
            <div class="pe-2 ">
              <p>
                ♡
              </p>
            </div>
            <h1 class="text-uppercase">
              hi! i'm laura
            </h1>
          </div>

          <!-- Left part: Paragraph about me -->
          <p class="pb-2">
            After spending three years in the UK as a flight attendant, I decided to pursue a new passion and turn my interest in technology into a career. 💻<br><br>

            I trained as a Full Stack Web Developer at Boolean and gained experience as a Java Backend Developer at VLC2, working with 
            <span class="text-pink fw-bolder">Java 21, Spring Boot, REST APIs, and MySQL databases</span>.
             I'm passionate about backend development and enjoy building applications, solving problems,
              and continuously expanding my technical skills.<br><br>

            <span class="text-decoration-underline fw-bolder">I'm currently looking for a Junior Backend Developer opportunity
            </span>, where I can contribute to real-world projects, collaborate with a development team, and continue growing as a developer.
             I also bring an international mindset, fluent English, and a strong determination to learn and contribute.🌟<br><br>

            In my free time, I enjoy music, playing guitar, reading, gaming… and watching too many
            adorable cat videos online! ;P
          </p>

          <!-- Resume button -->
          <div>
            <a href="/other/LauraOliveriCV.pdf" download>
              <button type="button" class="btn btn-outline text-uppercase">Resume</button>
            </a>
          </div>
        </div>

        <!-- Right part with pic -->
        <div class="col-md-6 col-12 text-center">
          <img src="/src/assets/images/me.jpg" alt="" class="polaroid">
        </div>
      </div>

    </div>
  </section>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

section {
  padding-top: 150px;
  color: $white;
  width: 100%;
  min-height: 100vh;
}

.polaroid {
  max-width: 335px;
  width: 100%;
  padding-top: 20px;
  transform: rotate(5deg);
}

.about_me {
  h1 {
    color: $pink;
    text-decoration: none;
    letter-spacing: 1.5px;
    font-family: 'VT323', sans-serif;
  }

  p {
    font-size: large;
  }

}

.btn-outline {
  font-family: $btn-font-family;
  font-weight: $btn-font-weight;
  padding: $btn-outline-padding-y $btn-outline-padding-x;
  border-radius: $btn-outline-border-radius;
  transition: $btn-outline-transition;
  letter-spacing: 1.5px;
  color: $white !important;
  background-color: transparent !important;
  border: 1.5px solid transparent !important; 
  position: relative;
  z-index: 1;
  cursor: pointer;

  // Aurora border effect
  &::before {
    content: '';
    position: absolute;
    inset: 0;
    border-radius: $btn-outline-border-radius;
    padding: 1.5px; 

    background: $aurora-gradient;
    background-size: 200% auto;
    background-position: 0% center;
    -webkit-mask: linear-gradient(#fff 0 0) content-box, linear-gradient(#fff 0 0);
    -webkit-mask-composite: xor;
            mask-composite: exclude;
            
    transition: background-position 0.4s ease;
    z-index: -1;
  }

  // Clear background
  &:hover, &.hover {
    color: $white !important;
    background-color: transparent !important;
    box-shadow: 0 0 20px rgba(#d91b8f, 0.35); 
    transform: translateY(-1px);

    &::before {
      background-position: 100% center; 
  }
  }
}

.text-pink {
  color: $pink;
}
</style>
