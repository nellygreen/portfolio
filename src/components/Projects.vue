<template>
    <section class="text-white mt-20" id="testimonials" data-aos="zoom-in">
        <h2 class="text-3xl font-bold text-secondary text-left mb-4 px-4 xl:pl-16 ">::::my__latest__projects:::</h2>
        <div class="p-4 xl:px-16">
            <Carousel v-bind="settings" :breakpoints="breakpoints">
                <Slide v-for="element in testimonials" :key="element.id">
                    <div class="carousel__item p4 my-2 ">
                        <div class="w-full mx-auto bg-treciary shadow-xl p-5 text-white font-light mb-6">
                            <div class="w-full flex mb-4 items-center">
                                <div class="overflow-hidden w-50 h-50">
                                    <img :src="element.image" alt="project image" loading="lazy">
                                </div>
                                <h6 class="ml-4 font-bold text-sm uppercase text-white">{{ element.fullName }}</h6>
                            </div>                            
                        </div>
                    </div>
                </Slide>
            </Carousel>
        </div>     

    </section>
</template>

<script setup>
import { ref } from 'vue';
import { Carousel, Navigation, Slide } from 'vue3-carousel';
import 'vue3-carousel/dist/carousel.css';
//Carousel settings
const settings =ref({
    itemsToShow:1,
    snapAlign:"center",
})

//Breakpoints
const breakpoints =ref({
    700:{
        itemsToShow:3,
        snapAlign:'center',
    },
    1024:{
        itemsToShow:5,
        snapAlign:'start'
    }
})

const testimonials=ref([
    {
        id:1,
        fullName:'Project 1',
        image:'src/assets/project_01.png'
    },
    {
        id:2,
        fullName:'Project 2',
        image:'src/assets/project_02.png'
    },
    {
        id:3,
        fullName:'Project 3',
        image:'src/assets/project_03.png'
    },
    {
        id:4,
        fullName:'Project 4',
        image:'src/assets/project_04.png'
    },
    {
        id:5,
        fullName:'Project 5',
        image:'src/assets/project_05.png'
    },
])
</script>
<style>
    .carousel__prev,.carousel__next {
        color: white !important;
    }
</style>