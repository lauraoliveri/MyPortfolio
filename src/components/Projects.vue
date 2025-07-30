<script>
export default {
  data() {
    return { 
      
    }
  }
}
</script>

<template>
  <section>
    <h2 class="py-5">
      PROJECTS
    </h2>

    <!-- Cards container -->
     <div class="d-flex justify-content-evenly">
      <div class="card_c  p-2">
        <div class="img_square">
          <img src="" alt="">
        </div>
        <div>
          <h4>
            PROGETTO 1
          </h4>
          <p>
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nam debitis aperiam itaque nobis consequuntur provident, iste eveniet eligendi porro voluptatem molestias inventore ipsam optio quo accusantium possimus officia. Doloremque, sequi.
          </p>
        </div>
      </div>

      <div class="card_c  p-2">
        <div class="img_square">
          <img src="" alt="">
        </div>
        <div>
          <h4>
            PROGETTO 1
          </h4>
          <p>
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nam debitis aperiam itaque nobis consequuntur provident, iste eveniet eligendi porro voluptatem molestias inventore ipsam optio quo accusantium possimus officia. Doloremque, sequi.
          </p>
        </div>
      </div>
      <div>

      </div>
     </div>
    <hr>
  </section>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

section {
  background-color: $custom_white;
  text-align: center;
}

h2, h4 {
  font-family: 'Relashionship of Melodrame', sans-serif;
}

.card_c {
  width: 500px;
  text-align: center;
}

.img_square {
  background-color: $yellow;
  width: 300px;
  height: 300px;
  text-align: center;
  padding: 10px;
}
</style>
