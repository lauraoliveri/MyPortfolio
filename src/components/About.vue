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
    <div class="container about_me">
      <div class="row">

        <!-- left part: description -->
        <div class="col-md-6 col-12">
         <div>
            <h1>
              ABOUT ME
            </h1>
          </div>

          <!-- paragraph about me -->
          <p class=" pb-2">
            Ciao! Sono una ragazza di 22 anni, curiosa e determinata, sempre pronta ad affrontare nuove sfide e crescere.<br><br>
            Dopo aver realizzato il mio sogno d’infanzia lavorando come hostess di volo, ho scoperto una nuova passione: l’informatica.<br>
            Questo mi ha portato a frequentare un corso intensivo di 700 ore in <strong>sviluppo front-end e back-end</strong>, durante il quale ho acquisito competenze solide e tanta voglia di continuare ad imparare.<br><br>
            Ora cerco un’opportunità per mettere in pratica ciò che ho appreso e continuare a crescere nel mondo dello sviluppo web.<br><br>
            Nel tempo libero mi rilasso tra musica, chitarra, letture, videogame… e un numero forse eccessivo di video di gattini su Internet :).
          </p>

          <!-- resume button -->
          <div>
            <button type="button" class="btn btn-outline">View Resume</button>
          </div>
        </div>

        <!-- right part with pic -->
        <div class="col-md-6 col-12 text-end">
          <img src="/src/assets/images/me.png" alt="">
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

// About me section

section{
  background-color: $black;
  color: $white;
  width: 100%;
  min-height: 100vh;
}


img {
  width: 335px;
  padding-top: 20px;
  transform: rotate(5deg);
}

.about_me {
  h1{
    color: $pink;
    text-decoration: none;
    font-family: 'VT323', sans-serif;
  }

  p{
    font-size: large;
  }

  @include underline-on-hover;
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

  &:hover {
    background-color: $btn-outline-hover-bg;
    color: $btn-outline-hover-color;
    border-color: $btn-outline-hover-border;
 
  }

}

</style>
