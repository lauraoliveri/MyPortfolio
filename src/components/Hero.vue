<script>
export default {
  data() {
    return {

    }
  }
}
</script>

<template>
  <div class="container-fluid px-0" id="home">
    <!-- Navbar with links -->

    <nav class="navbar navbar-expand-md py-3" data-bs-theme="dark">
      <div class="px-3 fw-bold d-md-none d-flex align-items-center">
        <img src="/src/assets/images/white_pink_flower.svg" class="w_p_flower">
        <div class="d-flex align-items-center ps-2">
          Laura's Portfolio
        </div>
      </div>
      <!-- Hamburger mobile -->
      <button class="navbar-toggler d-md-none ms-auto me-2" type="button" data-bs-toggle="collapse"
        data-bs-target="#mobileMenu" aria-controls="mobileMenu" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>

      <!-- Link -->
      <div class="collapse navbar-collapse" id="mobileMenu">
        <ul class="navbar-nav w-100 d-flex justify-content-evenly flex-md-row text-center align-items-center">
          <li class="nav-item d-md-none">❀</li>
          <li class="nav-item"><a class="nav-link fs-4 fw-semibold" href="#about">ABOUT</a></li>
          <li class="nav-item"><a class="nav-link fs-4 fw-semibold" href="#skills">SKILLS</a></li>
          <li class="nav-item"><a class="nav-link fs-4 fw-semibold" href="#projects">PROJECTS</a></li>
          <li class="nav-item"><a class="nav-link fs-4 fw-semibold" href="#contacts">CONTACTS</a></li>
          <li class="nav-item d-md-none">❀</li>
        </ul>
      </div>
    </nav>

    <!-- Introduction -->
    <div class="d-flex flex-column justify-content-center align-items-center" id="hello" style="height: 100vh;">
      <div class="hello-container text-center">
        <h1 class="hello-text">
          <span>H</span><span>E</span><span>L</span><span>L</span><span>O</span><span>!</span>
          <span>
            <img src="/src/assets/images/white_pink_flower.svg" alt="">
          </span>
        </h1>
      </div>

      <div id="my_name">
        I'm Laura S Oliveri
      </div>

      <div id="neon_text">
        Full-Stack Web Developer
      </div>
    </div>

    <!-- Section divider -->
    <div class="custom-shape-divider-bottom-1764679236">
      <svg data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120" preserveAspectRatio="none">
        <path
          d="M985.66,92.83C906.67,72,823.78,31,743.84,14.19c-82.26-17.34-168.06-16.33-250.45.39-57.84,11.73-114,31.07-172,41.86A600.21,600.21,0,0,1,0,27.35V120H1200V95.8C1132.19,118.92,1055.71,111.31,985.66,92.83Z"
          class="shape-fill"></path>
      </svg>
    </div>
  </div>

</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

#home {
  color: $white;
  width: 100%;
  min-height: 90vh;
  position: relative;
}

// Section divider 

.custom-shape-divider-bottom-1764679236 {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  overflow: hidden;
  line-height: 0;
}

.custom-shape-divider-bottom-1764679236 svg {
  position: relative;
  display: block;
  width: calc(100% + 1.3px);
  height: 18px;
}

.custom-shape-divider-bottom-1764679236 .shape-fill {
  fill: #1D1313;
}

// 
.navbar {
width: 100%;
  background-color: $black;
  text-align: center;
  height: 70px;
}

.navbar-collapse {


  &.collapse.show {
    background-color: $black; // When Hamburger menù is showed
    padding: 20px;
    z-index: 1;
  }
}

.w_p_flower {
  width: 30px;
  border-top: 50px;
}


ul {
  list-style: none;

  li {
    a {
      text-decoration: none;
      color: $pink;
      font-family: 'VT323', sans-serif;

      &:hover {
        transform: scale(0.9);
        color: $white;
      }
    }

  }

}

#my_name {
  font-size: 70px;

  /* Neon shadow */
  text-shadow:
    0 0 8px rgba($pink, 0.6),
    0 0 16px rgba($pink, 0.4),
    0 0 24px rgba($white, 0.15);
}

/*
Hello text Animation
*/

.hello-text span {
  display: inline-block;
  font-size: 100px;
  animation: hello 2s ease-in-out infinite;
}

.hello-text span:nth-child(1) {
  animation-delay: 0s;
}

.hello-text span:nth-child(2) {
  animation-delay: 0.2s;
}

.hello-text span:nth-child(3) {
  animation-delay: 0.4s;
}

.hello-text span:nth-child(4) {
  animation-delay: 0.6s;
}

@keyframes hello {

  0%,
  100% {
    transform: translateY(0);
  }

  50% {
    transform: translateY(-20px);
  }
}

/*
*/


/*
Neon animation
*/

@keyframes lights {
  0% {
    color: $white;
    text-shadow:
      0 0 1em rgba($pink, 0.2),
      0 0 0.125em rgba($pink, 0.3),
      -1em -0.125em 0.5em rgba($white, 0),
      1em 0.125em 0.5em rgba($pink, 0);
  }

  30% {
    color: lighten($pink, 25%);
    text-shadow:
      0 0 1em rgba($pink, 0.5),
      0 0 0.125em rgba($pink, 0.5),
      -0.5em -0.125em 0.25em rgba($white, 0.2),
      0.5em 0.125em 0.25em rgba($pink, 0.4);
  }

  40% {
    color: $white;
    text-shadow:
      0 0 1em rgba($pink, 0.5),
      0 0 0.125em rgba($white, 0.5),
      -0.25em -0.125em 0.125em rgba($white, 0.2),
      0.25em 0.125em 0.125em rgba($pink, 0.4);
  }

  70% {
    color: lighten($pink, 25%);
    text-shadow:
      0 0 1em rgba($pink, 0.5),
      0 0 0.125em rgba($pink, 0.5),
      0.5em -0.125em 0.25em rgba($white, 0.2),
      -0.5em 0.125em 0.25em rgba($pink, 0.4);
  }

  100% {
    color: $white;
    text-shadow:
      0 0 1em rgba($pink, 0.2),
      0 0 0.125em rgba($pink, 0.3),
      1em -0.125em 0.5em rgba($white, 0),
      -1em 0.125em 0.5em rgba($pink, 0);
  }
}

#neon_text {
  font-size: 100px;
  animation: lights 5s 750ms linear infinite;
  text-align: center;
}


// Media query mobile
@media (max-width: 576px) {

  #my_name {
    font-size: 40px;
  }

  .hello-text span {
    font-size: 80px;

  }

  #neon_text {
    font-size: 70px;
  }
  

}
</style>
