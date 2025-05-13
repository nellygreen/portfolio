<template>
  <div class="bg-[#7a7d79] min-h-screen">
    <NavBar />
    <HeroSection />
    <ServicesSection />
    <AboutSection />
    <ExperienceAndSkills />
    <Projects />
    <TestimonialSection />
    <ContactSection />  
    <FooterSection />
    <BackToTop />  
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
const Projects = defineAsyncComponent(()=>import('@/components/Projects.vue'));
const TestimonialSection = defineAsyncComponent(()=>import('@/components/TestimonialSection.vue'));
const FooterSection = defineAsyncComponent(()=>import('@/components/FooterSection.vue'));
const BackToTop = defineAsyncComponent(()=>import('@/components/BackToTop.vue'));


</script>