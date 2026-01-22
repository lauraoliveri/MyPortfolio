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

    <div class="text-center" id="icon">

      <!-- Divider -->
      <hr class="footer-divider"></hr>

      <!-- Message -->
      <div class=" p-5">
        Feel free to reach out via email or Linkedin :)
      </div>

      <!-- github -->
      <a href="https://github.com/lauraoliveri" class="pe-3 i-hover">
        <svg xmlns="http://www.w3.org/2000/svg" width="40" height="40" viewBox="0 0 40 40" fill="none" stroke="#fd7e98"
          stroke-width="1.25" stroke-linecap="round" stroke-linejoin="round"
          class="lucide lucide-github-icon lucide-github">
          <path
            d="M15 22v-4a4.8 4.8 0 0 0-1-3.5c3 0 6-2 6-5.5.08-1.25-.27-2.48-1-3.5.28-1.15.28-2.35 0-3.5 0 0-1 0-3 1.5-2.64-.5-5.36-.5-8 0C6 2 5 2 5 2c-.3 1.15-.3 2.35 0 3.5A5.403 5.403 0 0 0 4 9c0 3.5 3 5.5 6 5.5-.39.49-.68 1.05-.85 1.65-.17.6-.22 1.23-.15 1.85v4" />
          <path d="M9 18c-4.51 2-5-2-7-2" />
        </svg>
      </a>

      <!-- linkedin -->
      <a href="https://www.linkedin.com/in/laura-salvatrice-oliveri-48a5b7216/" class="pe-3 i-hover">
        <svg xmlns="http://www.w3.org/2000/svg" width="40" height="40" viewBox="0 0 40 40" fill="none" stroke="#fd7e98"
          stroke-width="1.25" stroke-linecap="round" stroke-linejoin="round"
          class="lucide lucide-linkedin-icon lucide-linkedin">
          <path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z" />
          <rect width="4" height="12" x="2" y="9" />
          <circle cx="4" cy="4" r="2" />
        </svg>
      </a>

      <!-- open gmail -->
      <a href="mailto:laurasalvatrice9@gmail.com?body=Hi!" class="pe-3 i-hover">
        <svg xmlns="http://www.w3.org/2000/svg" width="40" height="40" viewBox="0 0 40 40" fill="none" stroke="#fd7e98"
          stroke-width="1.25" stroke-linecap="round" stroke-linejoin="round"
          class="lucide lucide-mail-icon lucide-mail">
          <path d="m22 7-8.991 5.727a2 2 0 0 1-2.009 0L2 7" />
          <rect x="2" y="4" width="20" height="16" rx="2" />
        </svg>
      </a>
    </div>

    <!-- Copyrights -->
    <p class="copyrights text-center">
      © 2025 Laura Salvatrice Oliveri. All rights reserved.
    </p>
    
  </footer>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

footer {
  width: 100%;
  min-height: 210px;
  color: $white;
}

// Divider
.footer-divider {
  width: 30%;          
  height: 1px;      
  margin: 0 auto;      
  background: linear-gradient(
    to right, 
    transparent, 
    $pink,            
    transparent
  );
  box-shadow: 0 0 10px rgba(253, 126, 152, 0.4);
  opacity: 0.6;
  border: none;
}

.copyrights {
  color: $pink;
  font-size: 8px;
  opacity: 0.5;
  padding-top: 20px;
}

// Socials icons
#icon {
  padding-top: 10px;
}

.i-hover svg {
  color: $white;
  transition: color 0.3s ease, transform 0.3s ease;
}

.i-hover:hover svg {
  color: $pink;
  opacity: 0.5;
  transform: scale(1.1); // It becomes bigger
}

</style>
