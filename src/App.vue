<script setup>
import Navbar from './components/Navbar.vue';
import MyWelcome from './components/MyWelcome.vue';
import AboutMe from './components/AboutMe.vue';
import Projects from './components/Projects.vue';
import Contact from './components/Contact.vue';

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
  </header>

  <main>
    <section ref="homeSection"><MyWelcome /></section>
    <section ref="aboutSection"><AboutMe /></section>
    <section ref="projectsSection"><Projects /></section>
    <section ref="contactSection"><Contact /></section>
  </main>
</template>

<style scoped>
  
</style>
