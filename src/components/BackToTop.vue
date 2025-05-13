<template>i
    <button v-if="isVisible" @click="scrollToTop" class="fixed bottom-4 right-4 bg-transparent border-2 text-white
    rounded-full w-12 h-12 flex items-center justify-center cursor-pointer transition-opacity duration-300 hover:bg-secondary">
        <img class="w-7 h-7" src="https://img.icons8.com/ios-filled/100/ffffff/up.png">
    </button>
</template>
<script setup>
import { ref, onMounted, onUnmounted} from 'vue';
const isVisible =ref(false);
const handleScroll = ()=>{
    isVisible.value = window.scrollY > 300;
}
const scrollToTop = ()=>{
    window.scrollTo({top:0,behaviour:'smooth'})
}
onMounted(()=>{
    window.addEventListener('scroll',handleScroll)
})
onUnmounted(()=>{
    window.removeEventListener('scroll',handleScroll)
})
    
</script>