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

    <nav class="navbar navbar-expand-md py-3">
      <!-- Hamburger mobile -->
      <button class="navbar-toggler d-md-none ms-auto me-2" type="button" data-bs-toggle="collapse"
        data-bs-target="#mobileMenu" aria-controls="mobileMenu" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>

      <!-- Link -->
      <div class="collapse navbar-collapse" id="mobileMenu">
        <ul class="navbar-nav w-100 d-flex justify-content-center flex-md-row text-center">
          <li class="nav-item"><img src="/src/assets/images/white_pink_flower.svg" class="w_p_flower"></li>
          <li class="nav-item"><a class="nav-link fs-4 fw-semibold" href="#about">ABOUT</a></li>
          <li class="nav-item"><a class="nav-link fs-4 fw-semibold" href="#skills">SKILLS</a></li>
          <li class="nav-item"><a class="nav-link fs-4 fw-semibold" href="#projects">PROJECTS</a></li>
          <li class="nav-item"><a class="nav-link fs-4 fw-semibold" href="#footer">CONTACTS</a></li>
          <li class="nav-item"><img src="/src/assets/images/white_pink_flower.svg" class="w_p_flower"></li>
        </ul>
      </div>
    </nav>

    <!-- Introduction -->
    <div class="d-flex flex-column justify-content-center align-items-center" id="hello" style="height: 100vh;">
      <div class="hello-container text-center">
        <h1 class="hello-text">
          <span>H</span><span>e</span><span>l</span><span>l</span><span>o</span><span>!</span>
          <span>
            <img src="/src/assets/images/white_pink_flower.svg" alt="">
          </span>
        </h1>
      </div>

      <div id="my_name">
        I'm Laura S Oliveri
      </div>

      <div id="neon_text" >
        Full-Stack Web Developer
      </div>
    </div>

  </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

#home {
  color: $white;
  width: 100%;
  min-height: 100vh;
}

.navbar {
  background-color: $pink;
  text-align: center;
  height: 50px;
}

.w_p_flower {
  width: 30px;
  border-top: 50px;
}


// .bg_container .navbar {
//   background-color: rgba(255, 255, 255, 0);
// }

ul {
  list-style: none;

  li {
    margin-right: 100px;

    a {
      text-decoration: none;
      color: $black;
      font-family: 'VT323', sans-serif;

      &:hover {
        transform: scale(0.9);
      }
    }

  }

}

#hello {
  height: 80vh;

  h1 {

    font-size: 100px;
  }
}

/*
Hello text Animation
*/

.hello-text span {
  display: inline-block;
  font-size: 4rem;
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

#my_name {

  font-size: 50px;

}

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
}

</style>

