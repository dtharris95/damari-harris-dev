<script setup>

</script>

<template>
    <div class="welcome-container">
        <div class="logo-links">
            <img src="@/assets/linkedin.png" alt="" />
            <img src="@/assets/github.png" alt="" />
        </div>
        <div class="hello-world">
            <h1 class="intro">HELLO WORLD, I'M DAMARI</h1>
            <p class="intro-text">Eager to begin my career as a Web Developer, I  specialize in frontend web development, and blend creativity with traditional problem-solving to continuously expanding my  skillset.</p>
        </div>
    </div>
</template>

<style scoped>
    .welcome-container {
        display: flex;
    }

    .logo-links {
        background-color: #414B3B;
        height: 125px;
        width: 75px;
        margin-top: 100px;
    }

    .hello-world {
        color: #414B3B;
        margin: 0;
        padding: 0;
        text-align: center;
        padding-top: 5%;
        float: right;
    }

    .intro {
        font-family: "Raleway", sans-serif;
        font-size: 40px;
    }

    .intro-text {
        padding: 0 25%;
        font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
        font-size: 24px;
    }
</style>