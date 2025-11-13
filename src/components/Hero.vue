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
        <!-- Hamburger solo mobile -->
        <button
          class="navbar-toggler d-md-none ms-auto me-2"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#mobileMenu"
          aria-controls="mobileMenu"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>

        <!-- Link -->
        <div class="collapse navbar-collapse" id="mobileMenu">
          <ul class="navbar-nav w-100 d-flex justify-content-center flex-md-row text-center">
            <li class="nav-item"><a class="nav-link fs-4 fw-semibold" href="#about">ABOUT</a></li>
            <li class="nav-item"><a class="nav-link fs-4 fw-semibold" href="#skills">SKILLS</a></li>
            <li class="nav-item"><a class="nav-link fs-4 fw-semibold" href="#projects">PROJECTS</a></li>
            <li class="nav-item"><a class="nav-link fs-4 fw-semibold" href="#footer">CONTACTS</a></li>
          </ul>
        </div>
    </nav>

    <div class="d-flex justify-content-center align-items-center" id="code">
      <h1>
        function whoAmI() { <br>
          return "Full Stack Web Developer"; <br>
        }

      </h1>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

#home {
  background-color: $black;
  color: $white;
  width: 100%;
  min-height: 100vh;
}

.navbar {
  background-color: $pink;
  text-align: center;
}

.content {
  height: 60px;
}

#code{
  height: 80vh;
  
  h1 {
    font-family: 'VT323', sans-serif;
    color: $pink;
  }
}

// .bg_container .navbar {
//   background-color: rgba(255, 255, 255, 0);
// }

ul {
    list-style: none;

    li {
        margin-right: 100px;
        &:hover {
          transform: scale(0.9);
        }

        a {
            text-decoration: none;
            color: $black;
            font-family: 'VT323', sans-serif;  
        }
    }
     
}


</style>
