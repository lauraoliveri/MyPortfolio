<script>
export default {
  data() {
    return { 
      
    }
  }
}
</script>

<template>
  <footer id="footer">
      <!-- Links  -->
      <div class="pt-2 text-center" id="linkss">
        <ul >
          <li class="fs-5"><a href="#home">HOME</a></li>
          <li class="fs-5"><a href="#about">ABOUT</a></li>
          <li class="fs-5"><a href="#skills">SKILLS</a></li>
          <li class="fs-5"><a href="#projects">PROJECTS</a></li>
        </ul>
      </div>
    
        <div class="text-center" id="icon">
          <!-- github -->
          <a href="https://github.com/lauraoliveri" class="pe-3 i-hover">
            <i class="fa-brands fa-github fa-2xl"></i>
          </a>
          <!-- linkedin -->
          <a href="https://www.linkedin.com/in/laura-salvatrice-oliveri-48a5b7216/" class="pe-3 i-hover">
            <i class="fa-brands fa-linkedin fa-2xl"></i>
          </a>
          <!-- open gmail -->
          <a href="mailto:laurasalvatrice9@gmail.com?body=Hi!" class="pe-3 i-hover">
            <i class="fa-solid fa-inbox fa-2xl"></i>
          </a>
        </div>
        <p class="copyrights text-center">
            © 2025 Laura Salvatrice Oliveri. All rights reserved. 
        </p>
  </footer>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

footer {
  width: 100%;
  height: 210px;
  background-color: $black;
  color: $white;
}

.copyrights {
  color: $pink;
  font-size: 8px;
  opacity: 0.5;
  padding-top: 20px;
}


a {
  text-decoration: none;
  color: $pink;  
}

ul {
  list-style: none;
  padding: 0;
  margin: 0;
  text-align: center;

    li {
        :hover {
            color: $white;
        }

        a {
          text-decoration: none; 
        }
    }
     
}

#linkss{
  font-family: 'VT323', sans-serif;
   
}

#icon {
  padding-top: 20px;
}

.i-hover i {
  color: $pink;
  transition: color 0.3s ease, transform 0.3s ease;
}

.i-hover:hover i {
  color: $pink;
  opacity: 0.5;
  transform: scale(1.1); /* leggero ingrandimento */
}
</style>
