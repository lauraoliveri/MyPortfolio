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
            I’m a 22-year-old, <span class="text-pink fw-bolder">curious and determined</span> aspiring developer, always
            ready to learn and grow. 🚀<br><br>

            After fulfilling my childhood dream of working as a flight attendant, I discovered a new passion:
            computer science. 💻<br>
            This led me to complete an intensive 700-hour course in <span class="text-pink fw-bolder">front-end</span> and
            <span class="text-pink fw-bolder">back-end</span> development, where I gained solid skills and a strong desire to
            keep learning. I also completed a course in Java, further expanding my programming skillset.<br><br>

            <span class="text-decoration-underline fw-bolder">I’m now looking for my first professional opportunity in
              IT</span>, excited to apply my skills, contribute to real projects, and continue growing as a
            developer. 🌟<br><br>

            In my free time, I enjoy music, playing guitar, reading, gaming… and watching too many
            adorable cat videos online!
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
          <img src="/src/assets/images/me.png" alt="" class="polaroid">
        </div>
      </div>

    </div>
  </section>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

section {
  padding-top: 100px;
  color: $white;
  width: 100%;
  min-height: 90vh;
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
