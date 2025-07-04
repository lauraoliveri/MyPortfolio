<script>
export default {
  data() {
    return { 
      
    }
  }
}
</script>

<template>
  <div class="bg_container">

    

    <!-- Navbar with links -->
     
    <nav id="content">
        <div class="nav-container">
            <div class="nav-links mx-5">
                <ul class="d-flex me-5 justify-content-center">
                    <li class="fs-5 fw-semibold"><a href="#">ABOUT</a></li>
                    <li class="fs-5 fw-semibold"><a href="#">SKILLS</a></li>
                    <li class="fs-5 fw-semibold"><a href="#">CONTACTS</a></li>
                </ul>
            </div>
        </div>
    </nav>

  </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

.bg_container {
  background-image: url(../assets/images/8169822.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  width: 100%;
  height: 100vh; 
  overflow: hidden;
}

.bg_container #content {
  position: relative;
  z-index: 1;
  color: black;
  text-align: center;
  padding: 2rem;
}


.bg_container .navbar {
  background-color: rgba(255, 255, 255, 0);
}

h1 {
    font-family: 'Relashionship of Melodrame', sans-serif;
}

ul {
    list-style: none;

    li {

        margin-right: 100px;
        :hover {
            color: rgb(0, 0, 0, 0.5);
        }

        a {
            text-decoration: none;
            color: $yellow;  
        }
    }
     
}
</style>
