<script setup>

</script>

<template>
    <div class="about-container">
        <h1 class="about-heading">ABOUT ME</h1>
        <div class="about-section">
            <div class="about-subsection">
                <h2>Get to Know Me!</h2>
                <p>Originally from Columbus, OH, in 2023 I earned my Associate of Applied  Sciences in Computer Science from Columbus State Community College,  majoring in Web Development.
                    <br></br><br></br>
                    Now based in Cleveland, OH, I have spent the last six years thriving in my role at Amazon and am now excited to embark on my next chapter in Web Development.
                    <br></br><br></br>
                    I’m open to job opportunities where I can learn, grow, and collaborate, all while making a meaningful impact.</p>
            </div>
            <div class="skills-container">
                <h2>Skills</h2>
                <div class="skill-list">
                    <p class="skill">JavaScript</p>
                    <p class="skill">HTML</p>
                    <p class="skill">CSS</p>
                </div>
                <div class="skill-list">
                    <p class="skill">React</p>
                    <p class="skill">Vue</p>
                    <p class="skill">Git</p>
                </div>
                <div class="skill-list">
                    <p class="skill">GitHub</p>
                    <p class="skill">Responsive Design</p>
                    <p class="skill">Bootstrap</p>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .about-container {
        background-color: #414B3B;
        padding: 10% 0;
        width: 100vw;
        max-width: 100%;
        color: #D9D9D9;
    }

    .about-heading {
        text-align: center;
        color: #D9D9D9;
        font-size: 48px;
    }

    .about-section {
        display: flex;
        padding: 2%;
    }

    .about-subsection {
        width: 35%;
        padding: 0 10%;
    }

    .skills-container {
        width: 35%;
    }

    .skill-list {
        display: flex;
        justify-content: space-between;
    }

    .skill {
        background-color: #D9D9D9;
        color: #414B3B;
        font-weight: bold;
        padding: 10px 15px;
    }

    /* Extra small devices (phones, 600px and down) */
    @media only screen and (max-width: 600px) {

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

