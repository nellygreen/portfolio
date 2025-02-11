<template>
    <section class="text-white mt-20" id="services">
        <div class="px-4 xl:pl-16">
            <h2 class="text-3xl font-bold text-secondary mb-4">::::my services::::</h2>
        </div>
        <div class="py-8 px-4 sm:py-16 grid grid-cols-1 gap-6 pt-10 sm:grid-cols-2 md:gap-10 md:pt-12 lg:grid-cols-3">
            <div v-for="service in services" :key="service.id" data-aos="fade-up"
            class="px-8 py-12 rounded-xl bg-[#23001b] shadow-xl ">
                <div class="mx-auto h-24 text-center xl:h-28 xl:w-28">
                    <div class="">
                        <img :src="service.icon" alt="service icon" class="text-primary">
                    </div>
                </div>
                <div class="text-center">
                    <h3 class="pt-8 text-lg font-semibold uppercase text-primary">
                        {{ service.name }}
                    </h3>
                    <p class="text-grey pt-4 text-sm group-hover:text-white md:text-base">
                        {{ service.description }}
                    </p>
                </div>
            </div>
        </div>
    </section>
</template>
<script setup>
import {ref} from 'vue';
const services =ref([
    {
        id:1,
        icon: 'https://img.icons8.com/ios-filled/100/ffffff/google-code.png',
        name: 'UI/UX',
        description: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ex, ipsum.'
    },
    {
        id:2,
        icon: 'https://img.icons8.com/ios-filled/100/ffffff/google-code.png',
        name: 'FRONT-END',
        description: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ex, ipsum.'
    },
    {
        id:3,
        icon: 'https://img.icons8.com/ios-filled/100/ffffff/google-code.png',
        name: 'WEBGL',
        description: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ex, ipsum.'
    },
    {
        id:4,
        icon: 'https://img.icons8.com/ios-filled/100/ffffff/google-code.png',
        name: 'UNITY',
        description: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ex, ipsum.'
    },
    {
        id:5,
        icon: 'https://img.icons8.com/ios-filled/100/ffffff/google-code.png',
        name: '3D GRAPHICS',
        description: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ex, ipsum.'
    },
    {
        id:6,
        icon: 'https://img.icons8.com/ios-filled/100/ffffff/google-code.png',
        name: '2D GRAPHICS',
        description: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ex, ipsum.'
    }

])
</script>