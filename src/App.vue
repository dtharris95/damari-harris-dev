<script setup>
import Navbar from './components/Navbar.vue';
import MyWelcome from './components/MyWelcome.vue';
import AboutMe from './components/AboutMe.vue';
import Projects from './components/Projects.vue';
import Contact from './components/Contact.vue';
// import HelloWorld from './components/HelloWorld.vue'
// import TheWelcome from './components/TheWelcome.vue'

import { ref } from 'vue';
const homeSection = ref(null)
const aboutSection = ref(null)
const projectsSection = ref(null)
const contactSection = ref(null)

const sections = {
  home: homeSection,
  about: aboutSection,
  projects: projectsSection,
  contact: contactSection,
}

const scrollToSection = (sectionName) => {
  const section = sections[sectionName]?.value
  if (section) {
    section.scrollIntoView();
  }
}
</script>

<template>
  <header>
    <Navbar @scroll-to="scrollToSection" />
    <!-- <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />
    </div> -->
  </header>

  <main>
    <section ref="homeSection"><MyWelcome /></section>
    <section ref="aboutSection"><AboutMe /></section>
    <section ref="projectsSection"><Projects /></section>
    <section ref="contactSection"><Contact /></section>
    <!-- <TheWelcome /> -->
  </main>
</template>

<style scoped>
  


/* header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
} */
</style>
