<script setup>

</script>

<template>
    <div class="project-wrapper">
        <div>
            <h1 class="projects-heading">PROJECTS</h1><hr>
        </div>
        <!-- HARRIS KITCHEN TABLE -->
        <div class="projects-container">
            <div class="project">
                <a href="https://harriskitchentable.com" target="_blank"><img src="@/assets/HKTIcon.webp" alt="Image of my website, Harris Kitchen Table"></img></a>
                <div class="project-info">
                    <h2>Harris Kitchen Table</h2>
                    <p>Full-stack template website serving as proof-of-concept for potential freelance restaurant clients.</p>
                    <p>React | JavaScript | HTML | CSS | PocketBase</p>
                </div>
            </div>
            <!-- HINGE TO HARRIS -->
            <!-- <div class="project">
                <a></a>
                <img src="@/assets/city-vet-icon.webp" alt=""></img>
                <div class="project-info">
                    <h2>Hinge to Harris</h2>
                    <p>​My wedding website with details including the date, location, a form to RSVP, and a link to the registry, and details about the couple.​</p>
                    <p>WordPress | ouRSVP</p>
                </div>
            </div> -->
            <!-- CITY VETERINARY HOSPITAL -->
            <div class="project">
                <a></a>
                <img id="city-vet" src="@/assets/city-vet-icon.webp" alt="Fictional logo for my project, City Veterinary Hospital"></img>
                <div class="project-info">
                    <h2>City Veterinary Hospital (COMING SOON)</h2>
                    <p>Template veterinarian website serving as proof-of-concept for potential veterinarian clinic clients.</p>
                    <p>SvelteKit | JavaScript | HTML | CSS</p>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .project-wrapper {
        padding: 10% 0%;
    }

    .projects-heading {
        text-align: center;
        color: #414B3B;
        font-size: 48px;
    }

    .projects-container {
        text-align: center;
        padding: 0 10%;
    }

    .project {
        display: flex;
        padding: 5% 0;
        margin: 0 10%;
    }

    .project-info {
        padding: 0 10%;
        text-align: left;
        color: #414B3B;
    }

    hr {
        border: 2px solid #414B3B;
    }

    /* Extra small devices (phones, 600px and down) */
    @media only screen and (max-width: 600px) {
        .projects-heading {
            font-size: 28px;
        }

        .projects-container, .project {
            display: block;
        }

        .project-info {
            padding: 0 2%;
            text-align: center;
        }

        h2 {
            font-size: 20px;
        }
    }

    /* Small devices (portrait tablets and large phones, 600px and up) */
    @media only screen and (min-width: 601px) and (max-width: 767px) {
        .projects-heading {
            font-size: 32px;
            margin-bottom: 7%;
        }

        .projects-container, .project, .project-info {
            display: block;
            padding: 0;
            margin: 0;
            text-align: center;
        }

        .project-info {
            padding: 0 15%;
            margin: 5%;
        }

        h2 {
            font-size: 24px;
        }
    }

    /* Medium devices (landscape tablets, 768px and up) */
    @media only screen and (min-width: 768px) and (max-width: 991px) {
        .projects-heading {
            /* font-size: 32px; */
            margin-bottom: 7%;
        }

        .projects-container, .project, .project-info {
            display: block;
            padding: 0;
            margin: 0;
            text-align: center;
        }

        .project-info {
            padding: 0 20%;
            margin: 5%;
        }

        h2 {
            font-size: 24px;
        }
    }

    /* Large devices (laptops/desktops, 992px and up) */
    @media only screen and (min-width: 992px) and (max-width: 1199px) {
        #city-vet {
            height: 165px;
            width: 625px;
        }
    }

    /* Extra large devices (large laptops and desktops, 1200px and up) */
    @media only screen and (min-width: 1200px) {

    } 
</style>