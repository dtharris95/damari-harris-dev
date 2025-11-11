<script setup>

</script>

<template>
    <div class="about-container">
        <h1 class="about-heading">ABOUT ME</h1><hr>
        <div class="about-section">
            <div class="about-subsection">
                <h2>Get to Know Me!</h2>
                <p class="about-text">Originally from Columbus, OH, in 2023 I earned my Associate of Applied  Sciences in Computer Science from Columbus State Community College,  majoring in Web Development.</p>
                    <p class="about-text">Now based in Cleveland, OH, I have spent the last six years thriving in my role at Amazon and am now excited to embark on my next chapter in Web Development.</p>
                    <p class="about-text">I’m open to job opportunities where I can learn, grow, and collaborate, all while making a meaningful impact.</p>
                    <p class="about-text">Feel free to connect with me on <a id="linkedin-link" href="https://linkedin.com/in/damariharris" target="_blank"><u>LinkedIn</u></a>! If you have a job opportunity for me that you feel matches my skill set, please don't hesitate to reach out.</p>
                    <button @click="$emit('scroll-to', 'contact')" type="submit" id="submit">CONTACT</button>
            </div>
            <div class="skills-container">
                <h2>Skills</h2>
                <div class="skill-list">
                    <p class="skill">JavaScript</p>
                    <p class="skill">HTML</p>
                    <p class="skill">CSS</p>
                    <!-- <p class="skill"></p> -->
                </div>
                <div class="skill-list">
                    <p class="skill">React</p>
                    <p class="skill">Vue</p>
                    <p class="skill">Git</p>
                    <p class="skill">WordPress</p>
                </div>
                <div class="skill-list">
                    <p class="skill">GitHub</p>
                    <p class="skill">Responsive Design</p>
                    <p class="skill">Bootstrap</p>
                    <!-- <p class="skill"></p> -->
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

    .about-text {
        text-align: left;
    }

    .skills-container {
        width: 30%;
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
        border-radius: 3px;
    }

    #linkedin-link {
        text-decoration: none;
        color: #D9D9D9;
        font-weight: bolder;
    }

        #submit {
        margin: 5px 0;
        padding: 10px 45px;
        background-color: #D9D9D9;
        border: 1px solid #D9D9D9;
        border-radius: 5px;
        color: #414B3B;
        font-weight: bold;
        cursor: pointer;
        font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
        font-size: 14px;
    }

    /* Extra small devices (phones, 600px and down) */
    @media only screen and (max-width: 600px) {
        .about-heading {
            font-size: 28px;
        }

        h2 {
            font-size: 20px;
        }

        .about-section {
            display: block;
            text-align: center;
        }

        .about-subsection {
            display: block;
            width: 80%;
            margin-bottom: 15%;
        }

        .skills-container {
            display: block;
            width: 95vw;
            /* padding: 0 10%; */
        }

        .skill {
            padding: 5px 5px;
            margin: 10px;
            font-size: 12px;
        }

        .skill-list {
            align-items: center;
            justify-content: space-between;
            padding: 0 10%;
        }
    }

    /* Small devices (portrait tablets and large phones, 600px and up) */
    @media only screen and (min-width: 601px) and (max-width: 767px) {
        .about-heading {
            font-size: 32px;
        }

        .about-section {
            display: block;
            padding: 0;
        }

        .about-subsection {
            text-align: center;
            width: 100vw;
            padding: 0%;
            margin: 10% 0;
        }

        .skills-container {
            text-align: center;
            padding: 0;
            width: 100vw;
        }

        .skill-list {
            padding: 0 15%;
        }

        .about-text {
            margin: 20% 0;   
        }

        h2 {
            font-size: 24px;
        }

        p {
            padding: 0 10%;
        }
    }

    /* Medium devices (landscape tablets, 768px and up) */
    @media only screen and (min-width: 768px) and (max-width: 991px) {
        .about-section {
            display: block;
            padding: 0;
        }

        .about-subsection {
            text-align: center;
            width: 100vw;
            padding: 0%;
            margin: 10% 0;
        }

        .about-text {
            padding: 0 10%;
            text-align: left;
        }

        .skills-container {
            text-align: center;
            padding: 0;
            width: 100vw;
        }

        .skill-list {
            padding: 0 20%;
        }
    }

    /* Large devices (laptops/desktops, 992px and up) */
    @media only screen and (min-width: 992px) and (max-width: 1199px) {
        .about-subsection {
            width: 30%;
        }

        .skills-container {
            width: 30%;
        }

        .skill {
            margin: 10px;
        }
    }

    /* Extra large devices (large laptops and desktops, 1200px and up) */
    @media only screen and (min-width: 1200px) {

    } 

</style>

