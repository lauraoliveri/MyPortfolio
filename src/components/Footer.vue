<script>
export default {
  data() {
    return { 
      
    }
  }
}
</script>

<template>
  <footer class="d-flex justify-content-center">
    <div class="pt-2">
      
        <div  class="yellow_bg back_to">
          <a href="#about">
             &#8679; BACK TO TOP
          </a>
        </div>
       
        <div>
            <p class="copyrights pt-3 pb-2">
                © 2025 Laura Salvatrice Oliveri. All rights reserved. <br>
                Design & development by me.  <br>
                Icons by Lordicon, Flaticons, images by Freepik.

            </p>
        </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

footer {
  width: 100%;
  height: 180px;
  background-image: url(../assets/images/8169814.jpg);
  background-position: center center;    
  background-repeat: no-repeat;
  background-size: cover; 
  color: $custom_white;
}

.copyrights {
  color: black;
  font-size: smaller;
  opacity: 0.5;
}

.symbol {
  width: 100px;
  text-align: center;
}

.yellow_bg {
  color: black;
  background-color: $yellow;
  padding: 1px;
}

.back_to{
  width: 120px;
}

a {
  text-decoration: none;
  color: black;  
}
</style>
