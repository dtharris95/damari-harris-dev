<script setup>

</script>

<template>
    <div class="welcome-wrapper">
        <div class="logo-links">
            <a href="https://linkedin.com/in/damariharris" target="_blank"><img id="linkedin-logo" src="@/assets/linkedin.png" alt="linkedin logo"/></a>
            <a href="https://github.com/dtharris95" target="_blank"><img id="github-logo" src="@/assets/github.png" alt="github logo" /></a>
        </div>
        <div class="hello-world-container">
            <h1 class="intro">HELLO WORLD, I'M DAMARI</h1>
            <p class="intro-text">Eager to begin my career as a Web Developer, I  specialize in frontend web development, and blend creativity with traditional problem-solving to continuously expand my  skill set.</p>
        </div>
    </div>
</template>

<style scoped>
    .welcome-wrapper {
        display: flex;
        padding: 15% 0% 10% 0;
    }

    .logo-links {
        left: 0;
        background-color: #414B3B;
        height: 150px;
        width: 75px;
        margin-top: 75px;
        padding-top: 20px;
        text-align: center;    
    }

    #linkedin-logo {
        padding-bottom: 20px;
    }

    #github-logo {

    }

    .hello-world-container {
        color: #414B3B;
        margin: 0;
        padding: 0;
        text-align: center;
        padding-right: 5%;
    }

    .intro {
        font-size: 56px;
    }

    .intro-text {
        padding: 0 15%;
        font-size: 32px;
    }

    /* Extra small devices (phones, 600px and down) */
    @media only screen and (max-width: 600px) {
        .welcome-wrapper {
            /* display: block; */
        }

        .intro {
            font-size: 24px;
        }

        .intro-text {
            font-size: 16px;
        }

        .logo-links {
            height: 75px;
            width: 50px;
            padding-bottom: 2%;
        }

        #linkedin-logo {
            height: 25px;
            width: 25px;
        }

        #github-logo {
            height: 35px;
            width: 35px;
        }
    }

    /* Small devices (portrait tablets and large phones, 600px and up) */
    @media only screen and (min-width: 600px) {

    }

    /* Medium devices (landscape tablets, 768px and up) */
    @media only screen and (min-width: 768px) {

    }

    /* Large devices (laptops/desktops, 992px and up) */
    @media only screen and (min-width: 992px) {

    }

    /* Extra large devices (large laptops and desktops, 1200px and up) */
    @media only screen and (min-width: 1200px) {

    } 
</style>