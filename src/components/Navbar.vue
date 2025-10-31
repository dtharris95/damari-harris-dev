<script setup>

</script>

<template>
    <div class="navbar">
        <img src="@/assets/damari.png" alt="Image here" />
        <div class="nav-title">
            <h1>Damari Harris</h1>
        </div>
        <nav class="nav-tabs">
            <ul>
                <li>Home</li>
                <li>About</li>
                <li>Projects</li>
                <li>Contact</li>
            </ul>
        </nav>
    </div>
</template>

<style scoped>
    .navbar {
        margin: 0;
        display: flex;
        color: #414B3B;
        border-bottom: 2px #414B3B solid;
    }

    .nav-title {
        width: 75%;
        padding-left: 1%;
        font-family: "Raleway", sans-serif;
    }

    nav {
        width: 25%;
    }

    ul {
        display: flex;
        list-style-type: none;
        font-weight: bold;
        justify-content: space-between;
        padding: 5% 15px;
        font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    }

    img {
        width: 50px;
        height: 50px;
        border-radius: 5px;
        padding-top: 1%;
        padding-left: 2%;
    }


</style>