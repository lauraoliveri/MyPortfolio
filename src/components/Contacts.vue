<script>
export default {
    data() {
        return {

        }
    }
}
</script>

<template>
    <section id="contacts">
        <div class="container pb-5">

            <!-- Section Title -->
            <h1 class="fw-bold text-center pt-4 mb-5">
                Contacts
            </h1>

            <!-- Social links -->
            <div class="row g-4 justify-content-center">

                <!-- Email -->
                <div class="col-12 col-sm-6 col-md-4 d-flex justify-content-center">
                    <div class="text-center d-flex flex-column justify-content-between">
                        <div class="round_div px-5 py-1 mb-2">
                            Email
                        </div>
                        <p class="mb-0">
                            <a href="mailto:laurasalvatrice9@gmail.com?body=Hi!">
                                laurasalvatrice9@gmail.com
                            </a>
                        </p>
                    </div>
                </div>

                <!-- Linkedin -->
                <div class="col-12 col-sm-6 col-md-4 d-flex justify-content-center">
                    <div class="text-center d-flex flex-column justify-content-between">
                        <div class="round_div px-5 py-1 mb-2">
                            Linkedin
                        </div>
                        <p class="mb-0">
                            <a href="https://www.linkedin.com/in/laura-salvatrice-oliveri-48a5b7216/">
                                Laura Salvatrice Oliveri
                            </a>
                        </p>
                    </div>
                </div>

                <!-- Github -->
                <div class="col-12 col-sm-6 col-md-4 d-flex justify-content-center">
                    <div class="text-center d-flex flex-column justify-content-between">
                        <div class="round_div px-5 py-1 mb-2">
                            Github
                        </div>
                        <p class="mb-0">
                            <a href="https://github.com/lauraoliveri">
                                github.com/lauraoliveri
                            </a>
                        </p>
                    </div>
                </div>

            </div>
        </div>

    </section>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

section {
    background-color: $black;
    color: $white;
    min-height: 260px;
}

// Neon pills
.round_div {
    width: 250px;
    background-color: $white;
    color: $black;
    border-radius: 20px;
    text-align: center;

    /* Neon shadow */
    box-shadow:
        0 0 8px rgba($pink, 0.6),
        0 0 16px rgba($pink, 0.4),
        0 0 24px rgba($white, 0.15);
}

// Links
p {
    a {
        color: $white;
        text-decoration: none;

        &:hover {
            opacity: 0.8;
        }
    }
}
</style>
