<script>
export default {
  data() {
    return { 
      
    }
  }
}
</script>

<template>
  <footer>
    <div class="text-center pt-2">
        
        <div class="fs-4 fw-bold yellow_bg">
            &#8679;
        </div>
        <div  class="yellow_bg">
            BACK TO TOP
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
    height: 170px;
    background-image: url(../assets/images/8169814.jpg);
    background-position: center center;    
    background-repeat: no-repeat;
    background-size: cover; 
    color: $mainWhite;
}

.copyrights {
    color: black;
    font-size: smaller;
    opacity: 0.5;
}

.yellow_bg {
    color: black;
    background-color: $yellow;
    
}
</style>
