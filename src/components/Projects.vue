<script setup>

</script>

<template>
    <div class="project-wrapper">
        <div>
            <h1 class="projects-heading">PROJECTS</h1>
        </div>
        <div class="projects-container">
            <div class="project">
                <a href="https://harriskitchentable.com" target="_blank"><img src="@/assets/HKTIcon.png" alt=""></img></a>
                <div class="project-info">
                    <h2>Harris Kitchen Table</h2>
                    <p>Full-stack template website serving as proof-of-concept for potential freelance restaurant clients.</p>
                    <p>React | JavaScript | HTML | CSS | PocketBase</p>
                </div>
            </div>
            <div class="project">
                <img src="@/assets/city-vet-icon.png" alt=""></img>
                <div class="project-info">
                    <h2>City Veterinary Hospital (COMING SOON)</h2>
                    <p>Template veterinarian website serving as proof-of-concept for potential veterinarian clinic clients.</p>
                    <p>SvelteKit | JavaScript | HTML | CSS</p>
                </div>
            </div>
            <!-- <div class="project">
                <img src="@/assets/HKTIcon.png" alt=""></img>
                <div class="project-info">
                    <h2>Project Names</h2>
                    <p>Y'all wrong fam, THIS project rules.</p>
                </div>
            </div> -->
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

    /* Extra small devices (phones, 600px and down) */
    @media only screen and (max-width: 600px) {
        .projects-heading {
            font-size: 24px;
        }

        .projects-container, .project {
            display: block;
        }

        h2 {
            font-size: 20px;
            text-align: center;
        }

        p {
            text-align: center;
        }
    }

    /* Small devices (portrait tablets and large phones, 600px and up) */
    @media only screen and (min-width: 600px) and (max-width: 767px) {
        .projects-heading {
            font-size: 32px;
        }

        h2 {
            font-size: 24px;
        }
    }

    /* Medium devices (landscape tablets, 768px and up) */
    @media only screen and (min-width: 768px) and (max-width: 991px) {

    }

    /* Large devices (laptops/desktops, 992px and up) */
    @media only screen and (min-width: 992px) and (max-width: 1199px) {

    }

    /* Extra large devices (large laptops and desktops, 1200px and up) */
    @media only screen and (min-width: 1200px) {

    } 
</style>