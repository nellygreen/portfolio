<template>
  <div class="bg-[#111827] min-h-screen">
    <NavBar />
    <HeroSection />
  </div>  
</template>

<script setup>
import { defineAsyncComponent } from 'vue';
//improt components asynchronously
const NavBar = defineAsyncComponent(()=>import('@/components/NavBar.vue'));
const HeroSection = defineAsyncComponent(()=>import('@/components/HeroSection.vue'));
</script>