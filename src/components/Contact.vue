<script setup>
    import { ref } from 'vue';

    const isCardFlipped = ref(false);

    window.onload = function() {
        // Reset the form fields when the page loads
        document.getElementById("form").reset();
    };
</script>

<template>
    <div class="contact-wrapper">
        <h1 class="contact-heading">CONTACT</h1><hr>
        <p class="contact-text">I would love to hear from you! Please fill out the form down below, and I will get back to you as soon as possible.</p>

        <!-- BUSINESS CARD -->
        <!-- <button
            class="card-flip"
            :class="{ 'is-flipped': isCardFlipped }"
            type="button"
            :aria-pressed="isCardFlipped"
            :aria-label="isCardFlipped ? 'Show front of business card' : 'Show back of business card'"
            @click="isCardFlipped = !isCardFlipped"
        >
            <div class="card-flip-inner">
                <div class="card-flip-front">
                    <img class="biz-card" src="@/assets/biz-card-front.png" alt="Front of Damari Harris’s business card">
                </div>
                <div class="card-flip-back">
                    <img class="biz-card" src="@/assets/biz-card-back.png" alt="Back of Damari Harris’s business card">
                </div>
            </div>
        </button> -->

        <div contact-section>
            <div class="contact-container">
                <!-- MY CONTACT INFORMATION -->
                <div class="contact-info">
                    <div class="contact-info-row">
                        <!-- Icon provided by https://icons8.com/ -->
                        <img src="@/assets/email-img.png" alt="E-mail icon"></img>
                        <h2>Freelance</h2>
                        <p>dharris.webdev@gmail.com</p>
                        <!-- <h2>Employment</h2>
                        <p>dtharris95@gmail.com</p> -->
                    </div>
                    <div class="contact-info-row">
                        <!-- Icon provided by https://icons8.com/ -->
                        <img src="@/assets/location-img.png" alt="Location icon"></img>
                        <h2>Location</h2>
                        <p>Cleveland, OH</p>
                    </div>
                    <div class="contact-info-row">
                        <!-- Icon provided by https://icons8.com/ -->
                        <img src="@/assets/briefcase-img.png" alt="Briefcase icon representing my work availability"></img>
                        <h2>Availability</h2>
                        <p>Freelance</p>
                    </div>
                </div>

                <!-- CLIENT CONTACT FORM -->
                <div class="contact-form">
                    <form id="form" action="https://api.web3forms.com/submit" method="POST">
                        <input type="hidden" name="access_key" value="4abbf63d-8fbb-4a37-8056-137fe4582bd9">
                        <input type="hidden" name="subject" value="New Submission from Damari Harris Portfolio">
                        <!-- CUSTOM FORM DATA -->
                        <div class="form-row">
                            <label>Name</label>
                            <input type="text" id="name" class="contact-inputs" name="name" placeholder="Enter name..." required />
                        </div>
                        <div class="form-row">
                            <label>E-mail</label>
                            <input type="text" id="email" class="contact-inputs" name="email" placeholder="Enter e-mail..." required />
                        </div>
                        <div class="form-row">
                            <label>Subject</label>
                            <input type="text" id="subject" class="contact-inputs" name="subject" placeholder="Enter subject..." required />
                        </div>
                        <div class="form-row">
                            <label>Message</label>
                            <textarea id="message" class="contact-inputs" name="message" placeholder="Enter message..." required ></textarea>
                            <input type="hidden" name="redirect" value="https://web3forms.com/success" />
                            <button type="submit" id="submit" aria-label="Submit button for contact form">SUBMIT</button>
                        </div>
                        <!-- <div id="result"></div> -->
                    </form>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .contact-wrapper {
        background-color: #D9D9D9;
        padding: 10% 0%;
        color: #414B3B;
        text-align: center;
        /* box-shadow: 0px -10px 5px gray; */
    }

    .contact-container {
        display: grid;
        grid-template-columns: auto auto;
        margin: 0 0%;
        padding: 0 12%;
    }

    div.contact-info {
        display: flex;
        flex-direction: column;
        justify-content: space-evenly;
        gap: 2rem;
        background-color: #414B3B;
        color: #D9D9D9;
        border-radius: 5px;
        padding: 2rem 0;
        margin: 0 12%;
    }

    div.contact-info-row {
        border-radius: 5px;
        padding: 2% 0;
        margin: 0;
    }

    .contact-heading {
        text-align: center;
        color: #414B3B;
        font-size: 48px;
    }

    .contact-text {
        font-size: 24px;
        padding: 2% 15%;
    }

    /* Business Card Animation */
    .card-flip {
        display: block;
        position: relative;
        width: min(500px, calc(100vw - 2rem));
        aspect-ratio: 1.586 / 1;
        margin: 0 auto 2rem;
        padding: 0;
        border: 0;
        background: transparent;
        perspective: 1000px;
        cursor: pointer;
    }

    .card-flip-inner {
        position: relative;
        width: 100%;
        height: 100%;
        text-align: center;
        transition: transform 0.7s cubic-bezier(0.2, 0.7, 0.2, 1);
        transform-style: preserve-3d;
    }

    .card-flip:hover .card-flip-inner,
    .card-flip.is-flipped .card-flip-inner {
        transform: rotateY(180deg);
    }

    .card-flip-front, .card-flip-back {
        position: absolute;
        inset: 0;
        -webkit-backface-visibility: hidden;
        backface-visibility: hidden;
    }

    .biz-card {
        display: block;
        width: 100%;
        height: 100%;
        object-fit: contain;
    }

    .card-flip-back {
        transform: rotateY(180deg);
    }

    .card-flip:focus-visible {
        outline: 3px solid #414B3B;
        outline-offset: 6px;
        border-radius: 5px;
    }

    @media (prefers-reduced-motion: reduce) {
        .card-flip-inner {
            transition-duration: 0.01ms;
        }
    }

    .contact-form {
        background-color: #414B3B;
        color: #D9D9D9;
        border: 15px #414B3B solid;
        border-radius: 5px;
        padding: 7% 5%;
        text-align: left;
    }

    .form-row {
        padding: 1% 0;
    }

    input[type=text], textarea {
        width: 95%;
        padding: 15px 0;
        font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
        border: 1px solid #D9D9D9;
        border-radius: 5px;
    }

    textarea {
        height: 250px;
    }

    #name, #email, #subject, #message {
        padding: 10px;
        margin: 5px 0;
    }

    label {
        font-weight: 600;
    }
    
    #submit {
        margin: 5px 0;
        padding: 10px 45px;
        background-color: #D9D9D9;
        border: #D9D9D9;
        border-radius: 5px;
        color: #414B3B;
        font-weight: bold;
        cursor: pointer;
        font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
        font-size: 14px;
    }

    #submit:hover {
        background-color: #414B3B;
        color: #D9D9D9;
        border: 2px solid #D9D9D9;
        box-shadow: 0px 2px 5px;
    }

    hr {
        border: 2px solid #414B3B;
    }

    /* Extra small devices (phones, 600px and down) */
    @media only screen and (max-width: 600px) {
        .contact-container {
            display: grid;
            grid-template-columns: auto;
            padding: 0%;
            margin: 0;
        }
        
        .contact-heading {
            font-size: 28px;
        }

        .contact-text {
            font-size: 18px;
            padding: 0 8%;
        }

        .contact-form {
            margin: 0 5%;
        }

        div.contact-info {
            padding-inline: 0;
            margin: 5% 5%;
        }

        div.contact-info-row {
            padding: 1%;
            border-radius: 5px;
        }
    }

    /* Small devices (portrait tablets and large phones, 600px and up) */
    @media only screen and (min-width: 601px) and (max-width: 767px) {
        .contact-container {
            display: grid;
            grid-template-columns: auto;
            padding: 0;
            margin: 0;
            /* padding: 0 5%; */
        }

        .contact-heading {
            font-size: 32px;
        }

        .contact-text {
            font-size: 24px;
            /* padding: 0 7%; */
        }

        .contact-info {
            margin: 0 5%;
        }

        .contact-form {
            margin: 10% 12%;
        }
    }

    /* Medium devices (landscape tablets, 768px and up) */
    @media only screen and (min-width: 768px) and (max-width: 991px) {
        .contact-container {
            display: block;
        }
        
        .contact-text {
            padding: 0 8%;
        }

        div.contact-info {
            margin: 5% 1%;
            padding-inline: 1%;
        }

        .contact-form {
            width: 84%;
        }
    }

    /* Large devices (laptops/desktops, 992px and up) */
    @media only screen and (min-width: 992px) and (max-width: 1199px) {
        .contact-container {
            display: grid;
            grid-template-columns: auto auto;
            margin: 0 3%;
        }
        
        .contact-text {
            padding: 0 12% 2% 12%;
        }

        .contact-info {
            padding-inline: 4%;
        }

        .contact-info-row {
            margin: 0;
            justify-content: center;
        }

        .contact-form {
            margin: 0;
            width: 84%;
        }
    }

    /* Extra large devices (large laptops and desktops, 1200px and up) */
    @media only screen and (min-width: 1200px) and (max-width: 1440px) {
        .contact-info {
            padding-inline: 0;
            margin: 0;
        }

        .contact-form {
            width: 86%;
        }
    } 
</style>