<script setup>

</script>

<template>
    <div class="contact-wrapper">
        <h1 class="contact-heading">CONTACT</h1><hr>
        <p class="contact-text">I would love to hear from you! Please fill out the form below, and I will get back to you as soon as possible.</p>

        <form action="https://api.web3forms.com/submit" method="POST">
            <input type="hidden" name="access_key" value="4abbf63d-8fbb-4a37-8056-137fe4582bd9">
            <div class="form-row">
                <label>Name</label>
                <input type="text" id="name" class="contact-inputs" name="name" placeholder="Enter name..." required />
            </div>
            <div class="form-row">
                <label>E-mail</label>
                <input type="text" id="email" class="contact-inputs" name="email" placeholder="Enter e-mail..." required />
            </div>
            <div class="form-row">
                <label>Message</label>
                <textarea id="message" class="contact-inputs" name="message" placeholder="Enter message..." required ></textarea>
                <button type="submit" id="submit">SUBMIT</button>
            </div>
        </form>
    </div>
</template>

<style scoped>
    .contact-wrapper {
        background-color: #414B3B;
        padding: 10% 0%;
        color: #D9D9D9;
        text-align: center;
    }

    .contact-heading {
        text-align: center;
        color: #D9D9D9;
        font-size: 48px;
    }

    .contact-text {
        font-size: 24px;
        padding: 2%;
    }

    form {
        background-color: #D9D9D9;
        color: #414B3B;
        border: 15px #D9D9D9 solid;
        margin: 0 15%;
        /* padding: 15px 50px; */
        padding: 2% 5%;
        text-align: left;
    }

    .form-row {
        padding: 1% 0;
    }

    input[type=text], textarea {
        width: 95%;
        padding: 15px 0;
        font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    }

    textarea {
        height: 250px;
    }

    #name, #email, #message {
        padding: 10px;
        margin: 5px 0;
    }

    label {
        font-weight: 600;
    }
    
    #submit {
        margin: 5px 0;
        padding: 10px 45px;
        background-color: #414B3B;
        color: #D9D9D9;
        font-weight: bold;
        cursor: pointer;
        font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    }

    /* Extra small devices (phones, 600px and down) */
    @media only screen and (max-width: 600px) {
        .contact-heading {
            font-size: 28px;
        }

        .contact-text {
            font-size: 18px;
            padding: 0 8%;
        }

        form {
            margin: 0 5%;
        }
    }

    /* Small devices (portrait tablets and large phones, 600px and up) */
    @media only screen and (min-width: 601px) and (max-width: 767px) {
        .contact-heading {
            font-size: 32px;
        }

        .contact-text {
            font-size: 24px;
            padding: 0 7%;
        }
    }

    /* Medium devices (landscape tablets, 768px and up) */
    @media only screen and (min-width: 768px) and (max-width: 991px) {
        .contact-text {
            padding: 0 8%;
        }
    }

    /* Large devices (laptops/desktops, 992px and up) */
    @media only screen and (min-width: 992px) and (max-width: 1199px) {
        .contact-text {
            padding: 0 12% 2% 12%;
        }
    }

    /* Extra large devices (large laptops and desktops, 1200px and up) */
    @media only screen and (min-width: 1200px) {

    } 
</style>