<template>
  <div class="bg-[#7a7d79] min-h-screen">
    <NavBar />
    <HeroSection />
    <ServicesSection />
    <AboutSection />
    <ExperienceAndSkills />    
    
    <ContactSection /> 
    <BackToTop />    
    <Footer /> 
  </div>

</template>

<script setup>
import { defineAsyncComponent } from 'vue';
//import components asynchronously
const NavBar = defineAsyncComponent(()=>import('@/components/NavBar.vue'));
const HeroSection = defineAsyncComponent(()=>import('@/components/HeroSection.vue'));
const ServicesSection = defineAsyncComponent(()=>import('@/components/ServicesSection.vue'));
const AboutSection = defineAsyncComponent(()=>import('@/components/AboutSection.vue'));
const ContactSection = defineAsyncComponent(()=>import('@/components/ContactSection.vue'));
const ExperienceAndSkills = defineAsyncComponent(()=>import('@/components/ExperienceAndSkills.vue'));

const BackToTop = defineAsyncComponent(()=>import('@/components/BackToTop.vue'));
const Footer = defineAsyncComponent(()=>import('@/components/Footer.vue'));



</script>