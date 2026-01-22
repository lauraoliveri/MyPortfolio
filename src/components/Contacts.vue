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
                <div class="row justify-content-center">
                    <div class="col-12 col-md-4">

                        <!-- Social 1 -->
                        <div class="contact-item">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"
                                fill="none" stroke="#FD7E98" stroke-width="2" stroke-linecap="round"
                                stroke-linejoin="round" class="contact-icon">
                                <rect width="20" height="16" x="2" y="4" rx="2" />
                                <path d="m22 7-8.97 5.7a1.94 1.94 0 0 1-2.06 0L2 7" />
                            </svg>

                            <div class="round_div">Email</div>
                            <p><a href="mailto:laurasalvatrice9@gmail.com">laurasalvatrice9@gmail.com</a></p>
                        </div>
                    </div>

                    <!-- Social 2 -->
                    <div class="col-12 col-md-4">
                        <div class="contact-item">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"
                                fill="none" stroke="#FD7E98" stroke-width="2" stroke-linecap="round"
                                stroke-linejoin="round" class="contact-icon">
                                <path
                                    d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z" />
                                <rect width="4" height="12" x="2" y="9" />
                                <circle cx="4" cy="4" r="2" />
                            </svg>

                            <div class="round_div">Linkedin</div>
                            <p><a href="https://www.linkedin.com/..." target="_blank">Laura Salvatrice Oliveri</a></p>
                        </div>
                    </div>

                    <!-- Social 3 -->
                    <div class="col-12 col-md-4">
                        <div class="contact-item">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"
                                fill="none" stroke="#FD7E98" stroke-width="2" stroke-linecap="round"
                                stroke-linejoin="round" class="contact-icon">
                                <path
                                    d="M15 22v-4a4.8 4.8 0 0 0-1-3.5c3 0 6-2 6-5.5.08-1.25-.27-2.48-1-3.5.28-1.15.28-2.35 0-3.5 0 0-1 0-3 1.5-2.64-.5-5.36-.5-8 0C6 2 5 2 5 2c-.3 1.15-.3 2.35 0 3.5A5.403 5.403 0 0 0 4 9c0 3.5 3 5.5 6 5.5-.39.49-.68 1.05-.85 1.65-.17.6-.22 1.23-.15 1.85v4" />
                                <path d="M9 18c-4.51 2-5-2-7-2" />
                            </svg>

                            <div class="round_div">Github</div>
                            <p><a href="https://github.com/lauraoliveri" target="_blank">github.com/lauraoliveri</a></p>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Divider -->
        <div class="divider">
            . ݁₊ ⊹ . ݁˖ . ݁
        </div>

    </section>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

section {
    color: $white;
    min-height: 300px;
}

.contact-item {
    text-align: center;
    padding: 20px;
    display: flex;
    flex-direction: column;
    align-items: center;

    .contact-icon {
        margin-bottom: 12px;
        opacity: 0.9;
        filter: drop-shadow(0 0 5px rgba(253, 126, 152, 0.4));
    }

    .round_div {
        color: $pink;
        font-size: 0.85rem;
        font-weight: bold;
        text-transform: uppercase;
        letter-spacing: 2px;
        margin-bottom: 5px;
    }

    p {
        margin: 0;

        a {
            color: #ffffff;
            text-decoration: none;
            font-size: 1.1rem;
            opacity: 0.8;
            transition: all 0.3s ease;

            &:hover {
                opacity: 1;
                color: $blue;
                text-decoration: underline;
            }
        }
    }
}

.divider {
    height: 250px;
    display: flex;
    justify-content: center;
    align-items: center;
    color: $pink;
    font-family: monospace;
    font-size: 2rem;
    font-weight: 300;
    letter-spacing: 5px;
    opacity: 0.4;
    text-shadow: 0 0 15px rgba(253, 126, 152, 0.2);
}
</style>
