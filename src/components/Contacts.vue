<script>
export default {
  data() {
    return { 
      
    }
  }
}
</script>

<template>
  <section  id="contacts"> 
    <!-- Title -->
    <div>
      <h2 class="py-5">
        CONTATTI
      </h2>
    </div>

    <!-- Socials Icons and Links -->
    <div class="d-flex justify-content-around align-items-center socials">
      
        <!-- Email -->
        <div class="text-center">
          <lord-icon
            src="https://cdn.lordicon.com/gejrxhkx.json"
            trigger="hover"
            stroke="light"
            style="width:150px;height:150px">
          </lord-icon>

          <div>
            <a href="#">
              LAURASALVATRICE9@GMAIL.COM
            </a>
          </div>
        </div>
        

        <!-- Linkedin -->
        <div class="text-center">
          <lord-icon
            src="https://cdn.lordicon.com/ofrzywfo.json"
            trigger="hover"
            stroke="light"
            style="width:150px;height:150px">
          </lord-icon>

          <div>
            <a href="#">
              LINKEDIN
            </a>
          </div>
        </div>
       

        <!-- Github -->
        <div class="text-center">
          <lord-icon
            src="https://cdn.lordicon.com/acgiczyg.json"
            trigger="hover"
            stroke="light"
            style="width:150px;height:150px">
          </lord-icon>

          <div>
            <a href="#">
              GITHUB
            </a>
          </div>
        </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

section {
  background-color: $custom_white;
  text-align: center;
  height: 400px;
}

a {
  text-decoration: none;
  color: black;
}

h2 {
  font-family: 'VT323', sans-serif;
}

.socials {
  height: 200px;
}
</style>
