<template>
  <NavBar />
  <HeroSection />
  <FeatureSection />
  <ContactSection />
  <TourSection />
  <PartnersSection />
  <FootingSection />
</template>

<script>
import NavBar from './components/NavBar.vue';
import HeroSection from './components/HeroSection.vue';
import FeatureSection from './components/FeatureSection.vue';
import ContactSection from './components/ContactSection.vue';
import TourSection from './components/TourSection.vue';
import PartnersSection from './components/PartnersSection.vue';
import FootingSection from './components/FootingSection.vue';
export default {
    components: { NavBar, HeroSection, FeatureSection, ContactSection, TourSection, PartnersSection, FootingSection }
}
</script>

<style>
* {
  padding: 0;
  margin: 0;
  text-decoration: none;
  list-style: none;
  box-sizing: border-box;
  position: relative;
}
html {
  background-color: #F5F5F5;
}
</style>
