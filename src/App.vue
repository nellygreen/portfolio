<template>
  <div class="bg-[#35022a] min-h-screen">
    <NavBar />
    <HeroSection />
    <ServicesSection />
  </div>  
</template>

<script setup>
import { defineAsyncComponent } from 'vue';
//improt components asynchronously
const NavBar = defineAsyncComponent(()=>import('@/components/NavBar.vue'));
const HeroSection = defineAsyncComponent(()=>import('@/components/HeroSection.vue'));
const ServicesSection = defineAsyncComponent(()=>import('@/components/ServicesSection.vue'));
</script>