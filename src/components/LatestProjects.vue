<template>
    <section class="text-white mt-20" id="ptojects">
        <div class="px-4 xl:pl-16">
            <div class="mb-4 md:flex md:justify-between xl:pr-16">
                <h2 class="text-3xl font-bold text-secondary">::::my__latest__projects::::</h2>
                <div class="flex space-x-4 mb-4 mt-5 md:mt-0">
                    {{ project.image }}
                  
                </div>
            </div>            
         
            
        </div>
    </section>
</template>
<script setup>
import { ref, computed } from 'vue';

const Projects = ref([
    {
        id:1,
        category:'web development',
        image:'src/assets/image.png',
        title:'project 1',
        description:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Illo, odit.',
        technologies:['vue.js 3','vuex','Express'],
        gitURL:'',
        webURL:''
    },
    {
        id:2,
        category:'mobile app',
        image:'src/assets/image.png',
        title:'project 2',
        description:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Illo, odit.',
        technologies:['vue.js 3','vuex','Express'],
        gitURL:'',
        webURL:''
    },
    {
        id:3,
        category:'web development',
        image:'src/assets/image.png',
        title:'project 3',
        description:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Illo, odit.',
        technologies:['vue.js 3','vuex','Express'],
        gitURL:'',
        webURL:''
    }

]);



</script>