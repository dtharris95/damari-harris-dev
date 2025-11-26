<script setup>
import Navbar from './components/Navbar.vue';
import MyWelcome from './components/MyWelcome.vue';
import AboutMe from './components/AboutMe.vue';
import Projects from './components/Projects.vue';
import Services from './components/Services.vue';
import Contact from './components/Contact.vue';

import { ref } from 'vue';
const homeSection = ref(null)
const aboutSection = ref(null)
const projectsSection = ref(null)
const servicesSection = ref(null)
const contactSection = ref(null)

const sections = {
  home: homeSection,
  about: aboutSection,
  projects: projectsSection,
  services: servicesSection,
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
  </header>

  <main>
    <section ref="homeSection"><MyWelcome @scroll-to="scrollToSection" /></section>
    <section ref="aboutSection"><AboutMe @scroll-to="scrollToSection" /></section>
    <section ref="projectsSection"><Projects /></section>
    <section ref="servicesSection"><Services /></section>
    <section ref="contactSection"><Contact /></section>
  </main>
</template>

<style scoped>
  
</style>
