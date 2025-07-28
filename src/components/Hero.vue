<script>
export default {
  data() {
    return { 
      
    }
  }
}
</script>

<template>
  <div class="bg_container" id="about">
    <!-- Navbar with links -->
     
    <nav id="content">
        <div class="nav-container">
            <div class="nav-links mx-5">
                <ul class="d-flex  justify-content-center">
                    <li class="fs-5 fw-semibold"><a href="#about">ABOUT</a></li>
                    <li class="fs-5 fw-semibold"><a href="#skills">SKILLS</a></li>
                    <li class="fs-5 fw-semibold"><a href="#contacts">CONTACTS</a></li>
                </ul>
            </div>
        </div>
    </nav>


    <!-- About Me Section -->
     <section class="d-flex justify-content-between text-center">
      <div>
        <!-- Text -->
        <div>
          <h4 class="p-0">
            Hi!I'm
          </h4>
        </div>
        <div>
          <h1>
            Laura
          </h1>
        </div>

        <!-- Job -->
        <div>
          <h3 class="pb-4">
            Full-Stack Web Developer
          </h3>   
        </div>

        <!-- Pic -->
        <div id="my_pic">
          <img src="./../assets/images/my-pic.jpg" alt="Laura Oliveri">
        </div>
      </div>
      <div class="about_me_container">
        <div>
          <h2>
            ABOUT ME
          </h2>
        </div>

        <!-- paragraph about me -->
         <p>
          Ciao! Sono una ragazza di 22 anni, curiosa e determinata, sempre pronta ad affrontare nuove sfide e crescere.<br><br>
          Dopo aver realizzato il mio sogno d’infanzia lavorando come hostess di volo, ho scoperto una nuova passione: l’informatica.<br>
          Questo mi ha portato a frequentare un corso intensivo di 700 ore in <strong>sviluppo front-end e back-end</strong>, durante il quale ho acquisito competenze solide e tanta voglia di continuare ad imparare.<br><br>
          Ora cerco un’opportunità per mettere in pratica ciò che ho appreso e continuare a crescere nel mondo dello sviluppo web.<br><br>
          Nel tempo libero mi rilasso tra musica, chitarra, letture, videogame… e un numero forse eccessivo di video di gattini su Internet :).
        </p>
      </div>
     </section>
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

// About me section
h1 {
  font-family: 'Relashionship of Melodrame', sans-serif;
  font-size: 8rem;
  color: black;
}

h3 {
  color: $pink;
  text-decoration: underline;
}

#my_pic img {
  width: 335px;
  border-radius: 100%;
}

section {
  padding-left: 150px;
  padding-right: 150px;

}
.about_me_container {

  padding-top: 100px;
  width: 550px;
  

  h2{
    color: black;
    text-decoration: none;
    font-family: 'Relashionship of Melodrame', sans-serif;  
  }

  p{
    font-size: large;
  }

  &:hover{
    h2 {
      text-decoration: underline;
    }
  }
}
</style>
