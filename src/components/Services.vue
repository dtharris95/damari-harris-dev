<script setup>

</script>

<template>
    <div class="services-wrapper">
        <div>
            <h1 class="services-heading">SERVICES</h1><hr></hr>
            <p class="services-text">As a freelance developer, I offer several services to help you create and maintain a user-friendly website that reflects your brand.</p>
            <div class="services">
                <div class="service-block">
                <img src="@/assets/code.png"></img>
                    <h2>Custom Website Development</h2>
                    <p>Responsive sites using React, Vue, WordPress, built from scratch for your specific needs.</p>
                </div>
                <div class="service-block">
                    <img src="@/assets/wordpress.png"></img>
                    <h2>WordPress Development</h2>
                    <p>Elementor, plug-ins, custom themes, site customization.</p>
                </div>
                <div class="service-block">
                    <img src="@/assets/settings.png"></img>
                    <h2>Website Maintenance & Optimization</h2>
                    <p>Bug fixing, accessibility friendly, speed optimizing.</p>
                </div>
                <div class="service-block">
                    <img src="@/assets/hosting.png"></img>
                    <h2>Deployment & Hosting</h2>
                    <p>Deploying websites on DigitalOcean, Netlify.</p>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .services-wrapper {
        background-color: #414B3B;
        padding: 10% 5%;
        box-shadow: 0px -10px 5px gray,
        0 10px 5px gray;
    }

    .services-heading {
        text-align: center;
        color: #D9D9D9;
        font-size: 48px;
    }

    .services-text {
        text-align: center;
        color: #D9D9D9;
        font-size: 24px;
        margin: 2% 10%;
    }

    .services {
        color: #D9D9D9;
        display: grid;
        grid-template-columns: auto auto auto auto;
        justify-content: center;
        align-items: center;
        text-align: center;
    }

    .service-block {
        border-right: 3px solid #D9D9D9;
        border-left: 3px solid #D9D9D9;
        border-radius: 25px;
        padding: 25px 25px;
        margin: 25px 30px;
        height: 250px;
        width: 250px;
        box-shadow: 0 2px 5px;
    }

    /* .service-block:hover {
        box-shadow: 0 5px 10px;
    } */

         /* Extra small devices (phones, 600px and down) */
    @media only screen and (max-width: 600px) {
        .services-heading {
            font-size: 28px;
        }

        .services-text {
            font-size: 18px;
        }
        
        .services {
            display: grid;
            grid-template-columns: auto;
        }

        .service-block {
            border-top: 3px solid #D9D9D9;
            border-bottom: 3px solid #D9D9D9;
            border-left: none;
            border-right: none;
        }
    }

    /* Small devices (portrait tablets and large phones, 600px and up) */
    @media only screen and (min-width: 601px) and (max-width: 767px) {
        .services-heading {
            font-size: 32px;
        }

        .services-text {
            font-size: 24px;
        }

        .services {
            display: grid;
            grid-template-columns: auto;
        }
        
    }

    /* Medium devices (landscape tablets, 768px and up) */
    @media only screen and (min-width: 768px) and (max-width: 991px) {
        .services {
            display: grid;
            grid-template-columns: auto auto;
        }
    }

    /* Large devices (laptops/desktops, 992px and up) */
    @media only screen and (min-width: 992px) and (max-width: 1199px) {
        .services {
            display: grid;
            grid-template-columns: auto auto;
        }
    }

    /* Extra large devices (large laptops and desktops, 1200px and up) */
    @media only screen and (min-width: 1200px) and (max-width: 1440px) {
        .services {
            display: grid;
            grid-template-columns: auto auto;
        }
    } 
</style>