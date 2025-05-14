<template>
    <section class="text-white mt-20" id="testimonials" data-aos="zoom-in">
        <h2 class="text-3xl font-bold text-secondary text-left mb-4 px-4 xl:pl-16 ">::::testimonials::::</h2>
        <div class="p-4 xl:px-16">
            <Carousel v-bind="settings" :breakpoints="breakpoints">
                <Slide v-for="element in testimonials" :key="element.id">
                    <div class="carousel__item p4 my-2 ">
                        <div class="w-full mx-auto bg-treciary shadow-xl p-5 text-white font-light mb-6">
                            <div class="w-full flex mb-4 items-center">
                                <div class="overflow-hidden rounded-full w-10 h-10 bg-gray-50 border border-gray-200">
                                    <img :src="element.image" alt="testimonial image" loading="lazy">
                                </div>
                                <h6 class="ml-4 font-bold text-sm uppercase text-white">{{ element.fullName }}</h6>
                            </div>
                            <div class="w-full">
                                <p class="text-sm leading-tight">
                                    <span class="text-lg leading-none italic font-bold text-white mr-1"></span>
                                        {{ element.content }}
                                    <span class="text-lg leading-none italic font-bold text-white mr-1"></span>
                                </p>
                            </div>
                        </div>
                    </div>
                </Slide>
            </Carousel>
        </div>    
    </section>
    <footer class="mt-8 bottom-0 z-10 bg-secondary text-white" >
        <div class="container p-12 flex justify-between">
            <div class="text-white text-3xl font-bold">n:<span class="text-primary">::|::</span>:g</div>
            <p class="text-white text-left uppercase">2025 <span class="text-primary font-bold">|</span> All rights <span class="text-primary">reserved</span></p>
        </div>
    </footer>
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
        itemsToShow:2.5,
        snapAlign:'center',
    },
    1024:{
        itemsToShow:3,
        snapAlign:'start'
    }
})

const testimonials=ref([
    {
        id:1,
        fullName:'client 1',
        image:'src/assets/image.png',
        content:' Lorem ipsum dolor sit amet consectetur adipisicing elit. Nemo, quam.'
    },
    {
        id:2,
        fullName:'client 2',
        image:'src/assets/image.png',
        content:' Lorem ipsum dolor sit amet consectetur adipisicing elit. Nemo, quam.'
    },
    {
        id:3,
        fullName:'client 3',
        image:'src/assets/image.png',
        content:' Lorem ipsum dolor sit amet consectetur adipisicing elit. Nemo, quam.'
    },
    {
        id:4,
        fullName:'client 4',
        image:'src/assets/image.png',
        content:' Lorem ipsum dolor sit amet consectetur adipisicing elit. Nemo, quam.'
    },
    {
        id:5,
        fullName:'client 5',
        image:'src/assets/image.png',
        content:' Lorem ipsum dolor sit amet consectetur adipisicing elit. Nemo, quam.'
    },

])
</script>
<style>
    .carousel__prev,.carousel__next {
        color: white !important;
    }
</style>