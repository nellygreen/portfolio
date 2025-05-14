<template>
  <div class="bg-[#7a7d79] min-h-screen">
    <NavBar />
    <HeroSection />
    <ServicesSection />
    <AboutSection />
    <ExperienceAndSkills />   
    <ContactSection /> 
    <BackToTop />   
    <TestimonialSection />  
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
const TestimonialSection = defineAsyncComponent(()=>import('@/components/TestimonialSection.vue'));
const BackToTop = defineAsyncComponent(()=>import('@/components/BackToTop.vue'));
</script>