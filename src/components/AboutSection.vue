<template>
    <section class="text-white mt-18" id="about">
        <div class="absolute z-0 top-[93rem] inset-x-0 h-64 flex items-start">
            <div class=""></div>
        </div>
        <div class="md:grid md:grid-cols-2 gap-8 items-center py-8 px-4 xl:gap-16 sm:py-16 xl:px-16 z-1">
            <div data-aos="flip-right">
                <h2 class="text-3xl font-bold text-secondary text-left mb-8">::::my__education::::</h2>
                <div class="space-y-8 py-8">
                    <div v-for="element in education" :key="element.id"
                    class="flex items-center md:w-[80%] w-full rounded-xl bg-treciary shadow-lg">
                    <div class="w-1/4">
                        <img src="https://img.icons8.com/ios-glyphs/60/ffffff/graduation-cap--v1.png" alt="graduation">
                    </div>
                    <div class="w-3/4 pl-4">
                        <h3 class="text-2xl font-semibold uppercase text-transparent bg-clip-text bg-gradient-to-r from-primary to-secondary lg:text-xl">
                            {{ element.School }}
                        </h3>
                        <p class="text-white">{{ element.program }}</p>
                        <p class="text-white">{{ element.year }}</p>
                    </div>
                </div>
                </div>
            </div><!--.flip-right-->
            <div class="mt-4 md:mt-0 text-left flex flex-col z-10 h-full" data-aos="flop-right">
                <h2 class="text-3xl font-bold text-primary md:text-center text-left mb-4">
                    ::::more__about__me::::</h2>
                <p class="text-base lg:text-lg mt-8 py-8">
                    Lorem ipsum dolor sit, amet consectetur adipisicing elit. 
                    Numquam blanditiis eum perferendis ullam aut ex fuga quam, quo veritatis possimus illo recusandae dicta veniam, 
                    aperiam sit dolores amet deserunt tempore beatae reprehenderit explicabo porro pariatur totam expedita! Autem libero odit, 
                    animi obcaecati alias architecto tenetur tempora odit saepe impedit veritatis vero eligendi assumenda suscipit iusto possimus?
                </p>
                <div class="grid grid-cols-3 gap-4 max-w-lg pt-8">
                    <div class="text-center rounded-xl bg-treciary shadow-lg p-3">
                        <h3 class="text-white font-bold text-xl sm:text-2xl lg:text-3xl">+200</h3>
                        <p class="text-sm sm:text-base text-gray-300">Happy Clients</p>
                    </div>
                    <div class="text-center rounded-xl bg-treciary shadow-lg p-3">
                        <h3 class="text-white font-bold text-xl sm:text-2xl lg:text-3xl">+300</h3>
                        <p class="text-sm sm:text-base text-gray-300">Project</p>
                    </div>
                    <div class="text-center rounded-xl bg-treciary shadow-lg p-3">
                        <h3 class="text-white font-bold text-xl sm:text-2xl lg:text-3xl">+5</h3>
                        <p class="text-sm sm:text-base text-gray-300">Years of Experience</p>
                    </div>
                </div>                 
            </div>
        </div>
    </section>
</template>
<script setup>
import { ref } from 'vue';
const education=ref([
    {
        id:1,
        School:'school 1',
        program:'Software Engineer',
        year:'2022'
    },
    {
        id:2,
        School:'school 2',
        program:'Sofwware Engineer',
        year:'2020'
    }
])
</script>