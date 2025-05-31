<template>
    <Splide :options="options">
        <SplideSlide v-for="image in images" :key="image.id">
            <img :src="image.src" alt="Slide" />
        </SplideSlide>
    </Splide>
</template>
  
<script setup>
    import '@splidejs/vue-splide/css';
    import { Splide, SplideSlide } from '@splidejs/vue-splide';
    // importação das imagens para o array de imagens
    import image1 from '@/assets/images/AtleticaPanterao.jpeg';

    const images = [
        {id:1, src: image1, alt:'Atlética Panterão'},
        {id:2, src: image1, alt:'Atlética Panterão'},
        {id:3, src: image1, alt:'Atlética Panterão'},
        {id:4, src: image1, alt:'Atlética Panterão'},
    ]
    
    const options = {
        type: 'loop',
        perPage: 1,
        focus: 'center',
        padding: { right: '5rem', left: '5rem' },
        gap: '1rem',
        autoplay: true,
        pauseOnHover: true,
        arrows: true,
        pagination: true,
    };
</script>
  
<style scoped>
    img {
        width: 100%;
        border-radius: 1rem;
    }
</style>
  