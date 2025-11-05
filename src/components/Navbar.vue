<script setup>
    
</script>

<template>
    <div class="navbar">
        <img src="@/assets/damari-icon.png" alt="Image here" />
        <div class="nav-title">
            <h1>Damari Harris</h1>
        </div>
        <nav>
            <ul>
                <button @click="$emit('scroll-to', 'home')">Home</button>
                <button @click="$emit('scroll-to', 'about')">About</button>
                <button @click="$emit('scroll-to', 'projects')">Projects</button>
                <button @click="$emit('scroll-to', 'contact')">Contact</button>
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
        /* font-size: 20px; */
        width: 75%;
        padding-left: 1%;
    }

    ul {
        display: flex;
        list-style-type: none;
        justify-content: space-between;
        padding: 5%;
    }

    img {
        width: 50px;
        height: 50px;
        /* border-radius: 5px; */
        padding-top: 1%;
        padding-left: 2%;
    }

    button {
        color: #D9D9D9;
        font-size: 16px;
        background: none;
        border: none;
        font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
        font-weight: bold;
        cursor: pointer;
    }

     /* Extra small devices (phones, 600px and down) */
@media only screen and (max-width: 600px) {
    .navbar {
        width: 100vw;
    }

    .nav-title {
        font-size: 12px;
        padding: 0 3%;
    }

    ul {
        display: none;
    }
}

/* Small devices (portrait tablets and large phones, 600px and up) */
@media only screen and (min-width: 600px) and (max-width: 767px) {
    /* img {
      padding-top: 2.5%;  
    } */

    ul {
        margin-right: 25px;
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