<template>
    <section class="text-white mt-18" id="skills">
        <div class="absolute right-0 top-[110rem] h-full w-full justify-end">
            <span class="flex opacity-20">
                <span class="w-16 h-32 rounded-l-full flex bg-primary blur-2xl"></span>
                <span class="w-16 h-32 rounded-r-full flex bg-secondary blur-2xl mt-14"></span>
            </span>
        </div>
        <div class="md:grid md:grid-cols-2 gap-8 items-center py-8 px-4 xl:gap-16 xl:px-16">
            <div class="mt-4 md:mt-0 text-left flex flex-col z-10 h-full w-[80%]">
                <h2 class="text-3xl font-bold text-secondary text-left mb-4">
                    ::::my__skills::::
                </h2>
                <div class="mt-8" v-for="skill in Skills" :key="skill.id">
                    <div class="flex items-end justify-between" data-aos="fade-right">
                        <h4 class="font-semibold uppercase text-white">
                            {{ skill.name }}
                        </h4>
                        <h3 class="text-2xl font-bold text-white">{{ skill.width }}</h3>
                    </div>
                    <div class="mt-2 h-1 w-full bg-treciary rounded-full">
                        <div class="h-1 rounded-full bg-primary" :style="`width :${skill.width}`"></div>
                    </div>
                </div>                
            </div>
            <div data-aos="flip-left">
                <h2 class="text-3xl font-bold text-secondary text-left mb-8 md:text-center md:mt-0 mt-0">::::my__experience::::</h2>
                <div class="space-y-8 py-8" data-aos="fade-left">
                    <div v-for="element in Experiences" :key="element.id"
                    class="flex items-center rounded-xl p-4 bg-treciary shadow-lg"
                    >
                        <div class="w-1/4">
                            <img src="https://img.icons8.com/ios-filled/100/ffffff/lawyer.png" alt="lawyer">
                        </div>
                        <div class="w-3/4 pl-4">
                            <h3 class="text-2xl font-semibold uppercase text-primary bg-clip-text">
                                {{ element.role }}
                            </h3>
                            <p class="text-white">{{ element.company }}</p>
                            <p class="text-white">{{ element.date }}</p>
                        </div>

                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<script setup>
import { ref } from 'vue';
const Skills =ref([
    {
        id:1,
        name:'Html & CSS',
        width:'85%'
    },
    {
        id:2,
        name:'Python',
        width:'70%'
    },
    {
        id:3,
        name:'Javascript',
        width:'95%'
    },
    {
        id:4,
        name:'Figma',
        width:'90%'
    }
]);

const Experiences =ref([
    {
        id:1,
        role:'Software Engeneer',
        company:'Microsoft',
        date:'Mar 2023 - September 2024'
    },
    {
        id:2,
        role:'Software Engeneer',
        company:'Google',
        date:'Mar 2024 - September 2025'
    }
])
</script>