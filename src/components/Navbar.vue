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
        <div class="d-flex align-items-center ps-2">
          Laura's Portfolio
        </div>
      </div>
      
      <!-- Hamburger mobile -->
      <button class="navbar-toggler d-md-none ms-auto me-2" type="button" data-bs-toggle="collapse"
        data-bs-target="#mobileMenu" aria-controls="mobileMenu" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>

      <!-- Link for navigating -->
      <div class="collapse navbar-collapse" id="mobileMenu">
        <ul class="navbar-nav w-100 d-flex justify-content-evenly flex-md-row text-center align-items-center">
          <li class="nav-item d-md-none">❀</li>
          <li class="nav-item"><a class="nav-link fs-5 fw-semibold text-uppercase" href="#about">ABOUT</a></li>
          <li class="nav-item"><a class="nav-link fs-5 fw-semibold text-uppercase" href="#skills">SKILLS</a></li>
          <li class="nav-item"><a class="nav-link fs-5 fw-semibold text-uppercase" href="#projects">PROJECTS</a></li>
          <li class="nav-item"><a class="nav-link fs-5 fw-semibold text-uppercase" href="#contacts">CONTACTS</a></li>
          <li class="nav-item d-md-none">❀</li>
        </ul>
      </div>
      
    </nav>
  </div>

</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

#home {
  color: $white;
  width: 100%;
}

.navbar {
  width: 70%;            
  max-width: 1200px;      
  margin: 25px auto;      
  border-radius: 50px;    
  height: 50px;
  left: 0; right: 0;     
  z-index: 1000;
  position: fixed;
  background: rgba(230, 205, 210, 0.05) !important; 
  backdrop-filter: blur(12px) saturate(150%);
  -webkit-backdrop-filter: blur(12px) saturate(150%);
  box-shadow: 0 1px 30px rgba(0, 0, 0, 0.205);

}

// Mobile navbar
.navbar-collapse {
  &.collapse.show {
   
    background: rgba(26, 11, 30, 0.98) !important;
    backdrop-filter: blur(10px);
    -webkit-backdrop-filter: blur(10px);
    border-radius: 20px;
    margin-top: 15px;
    padding: 20px;
    border: 1px solid rgba($pink, 0.5); 
    box-shadow: 0 10px 40px rgba(0, 0, 0, 0.8);
  }
}

ul {
  list-style: none;

  li {
    a {
      text-decoration: none;
      letter-spacing: 2px; 
      color: rgba($white, 0.9);
      font-family: 'VT323', sans-serif;
      transition: transform 0.25s cubic-bezier(0.4, 0, 0.2, 1), color 0.2s ease, text-shadow 0.2s ease;
      user-select: none;

      &:hover {
        transform: scale(0.9);
        color: $white;
        transform: translateY(-1px) scale(1.03);
      }
    }

  }

}

</style>
