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
            <p class="intro-text">I'm a front-end Web Developer who enjoys bringing ideas to life! I'm eager to apply my skills and grow continuously through real-world opportunities.</p>
            <button @click="$emit('scroll-to', 'projects')" type="submit" id="submit">PROJECTS</button>
        </div>
        <!-- Logos placement on mobile devices -->
        <div class="logo-links-responsive">
            <!-- <div> -->
            <a href="https://linkedin.com/in/damariharris" target="_blank"><img id="linkedin-logo" src="@/assets/linkedin.png" alt="linkedin logo"/></a>
            <!-- </div>
            <div> -->
            <a href="https://github.com/dtharris95" target="_blank"><img id="github-logo" src="@/assets/github.png" alt="github logo" /></a>
            <!-- </div> -->
        </div>
    </div>
</template>

<style scoped>
    .welcome-wrapper {
        display: flex;
        padding: 18% 0% 17% 0;
        text-align: center;
    }

    .logo-links {
        left: 0;
        background-color: #414B3B;
        height: 150px;
        width: 75px;
        margin-top: 50px;
        padding-top: 20px;
        /* text-align: center;     */
    }

    .logo-links-responsive {
        display: none;
    }

    #linkedin-logo {
        padding-bottom: 20px;
    }

    /* #github-logo {

    } */

    .hello-world-container {
        color: #414B3B;
        margin: 0;
        padding: 0;
        text-align: center;
        padding-right: 5%;
    }

    .intro {
        font-size: 56px;
        font-weight: 800;
    }

    .intro-text {
        padding: 0 18%;
        font-size: 28px;
    }

    #submit {
        margin: 5px 0;
        padding: 15px 45px;
        background-color: #414B3B;
        color: #D9D9D9;
        font-weight: bold;
        cursor: pointer;
        font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    }

    /* Extra small devices (phones, 600px and down) */
    @media only screen and (max-width: 600px) {
        .welcome-wrapper {
            display: block;
            padding: 45% 0 35% 0;
        }

        .intro {
            font-size: 28px;
            text-align: center;
            padding: 0 15%;
        }

        .intro-text {
            font-size: 16px;
            text-align: center;
            padding: 0 10%;
        }

        .logo-links {
            display: none;
        }

        .logo-links-responsive {
            display: grid;
            grid-template-columns: auto auto;
            background-color: #414B3B;
            align-items: center;
            margin: 5% 38%;
        }

        #linkedin-logo {
            height: 25px;
            width: 25px;
            padding: 7px 6px;
        }

        #github-logo {
            height: 35px;
            width: 35px;
        }

        .hello-world-container {
            padding-right: 0;
        }

        #submit {
            padding: 10px 40px;
        }
    }

    /* Small devices (portrait tablets and large phones, 600px and up) */
    @media only screen and (min-width: 601px) and (max-width: 767px) {
        .welcome-wrapper {
            padding: 15% 0 5% 0;
        }

        .hello-world-container {
            padding-right: 10%;
        }

        .intro {
            font-size: 32px;
        }

        .intro-text {
            padding: 0 5%;
            font-size: 24px
        }

        .logo-links {
            margin: 7% 0;
            height: 120px;
        }

        #linkedin-logo {
            margin: 15% 0;
            padding: 3% 0;
            height: 35px;
            width: 35px;
        }

        #github-logo {
            height: 50px;
            width: 50px;
        }
    }

    /* Medium devices (landscape tablets, 768px and up) */
    @media only screen and (min-width: 768px) and (max-width: 991px) {
        .welcome-wrapper {
            padding: 40% 0 30% 0;
        }

        .intro {
            font-size: 48px;
        }

        .intro-text {
            font-size: 24px;
            padding: 0 5%;
        }

        .logo-links {
            margin: 7% 0;
            height: 120px;
        }

        #linkedin-logo {
            margin: 15% 0;
            padding: 0% 0;
            height: 35px;
            width: 35px;
        }

        #github-logo {
            height: 50px;
            width: 50px;
        }
    }

    /* Large devices (laptops/desktops, 992px and up) */
    @media only screen and (min-width: 992px) and (max-width: 1199px) {
        .welcome-wrapper {
            padding: 15% 0 5% 0;
        }

        .logo-links {
            margin: 10% 0;
        }
    }

    /* Extra large devices (large laptops and desktops, 1200px and up) */
    @media only screen and (min-width: 1200px) {

    } 
</style>