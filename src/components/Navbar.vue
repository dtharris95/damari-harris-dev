<script setup>
    
</script>

<template>
    <div class="navbar">
        <img src="@/assets/my-icon.webp" alt="Profile photo" />
        <div class="nav-title">
            <h1>Damari Harris</h1>
        </div>
        <nav>
            <ul>
                <li @click="$emit('scroll-to', 'home')">Home</li>
                <li @click="$emit('scroll-to', 'about')">About</li>
                <li @click="$emit('scroll-to', 'projects')">Projects</li>
                <li @click="$emit('scroll-to', 'contact')">Contact</li>
            </ul>
        </nav>
    </div>
</template>

<style scoped>
    .navbar {
        top: 0;
        left: 0;
        margin: 0;
        display: flex;
        border-bottom: 2px #D9D9D9 solid;
        position: fixed;
        width: 100vw;
        color: #D9D9D9;
        background-color: #414B3B;
    }

    .nav-title {
        font-size: 15px;
        width: 75%;
        padding-left: 1%;
    }

    nav {
        padding-right: 8%;
    }

    ul {
        display: flex;
        list-style-type: none;
        justify-content: space-between;
        padding: 6% 0;
    }

    img {
        width: 50px;
        height: 50px;
        padding-top: 0.75%;
        padding-left: 4%;
    }

    li {
        color: #D9D9D9;
        font-size: 16px;
        background: none;
        border: none;
        font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
        font-weight: bold;
        cursor: pointer;
        padding: 0 2%;
        padding-right: 1%;
    }

     /* Extra small devices (phones, 600px and down) */
    @media only screen and (max-width: 600px) {
        .navbar {
            width: 100vw;
            position: absolute;
        }

        .nav-title {
            font-size: 10px;
            padding: 1% 3%;
        }

        ul {
            display: none;
        }
    }

    /* Small devices (portrait tablets and large phones, 600px and up) */
    @media only screen and (min-width: 601px) and (max-width: 767px) {
        img {
        padding-top: 2.5%;  
        }

        nav {
            padding-right: 3%;
        }
    }

    /* Medium devices (landscape tablets, 768px and up) */
    @media only screen and (min-width: 768px) and (max-width: 991px) {
        img {
            padding-top: 1.5%;
            padding-left: 2%;
        }

        nav {
            padding-right: 5%;
        }
    }

    /* Large devices (laptops/desktops, 992px and up) */
    @media only screen and (min-width: 992px) and (max-width: 1199px) {
        img {
            padding-top: 1.5%;
        }

        nav {
            padding-right: 7%;
        }
    }

    /* Extra large devices (large laptops and desktops, 1200px and up) */
    @media only screen and (min-width: 1200px) {

    } 

</style>