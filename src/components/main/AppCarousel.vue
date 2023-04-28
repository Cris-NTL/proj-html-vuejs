<script>
import { VueperSlides, VueperSlide } from 'vueperslides';
import 'vueperslides/dist/vueperslides.css';

export default {
    name: 'AppCarousel',

    components: {
        VueperSlides,
        VueperSlide,
    },

    data: () => ({
        slides: [
            {
                title: 'High level of efficiency and scientific teaching methods',
                content: 'I am free to learn at my own pace, follow my own schedule and choose the subject i want to learn from the syllabus. Great study portal fro people like me.',
                // img: './src/assets/img/testimonial-avata-01.jpg',
                name: 'Mina Hollace',
                role: '/ Freelancer',
            },
            {
                title: 'High level of efficiency and scientific teaching methods',
                content: 'I am free to learn at my own pace, follow my own schedule and choose the subject i want to learn from the syllabus. Great study portal fro people like me.',
                // img: './src/assets/img/testimonial-avata-02.jpg',
                name: 'Mina Hollace',
                role: '/ Freelancer',
            },
            {
                title: 'High level of efficiency and scientific teaching methods',
                content: 'I am free to learn at my own pace, follow my own schedule and choose the subject i want to learn from the syllabus. Great study portal fro people like me.',
                // img: './src/assets/img/testimonial-avata-03.jpg',
                name: 'Mina Hollace',
                role: '/ Freelancer',
            },
            {
                title: 'High level of efficiency and scientific teaching methods',
                content: 'I am free to learn at my own pace, follow my own schedule and choose the subject i want to learn from the syllabus. Great study portal fro people like me.',
                // img: './src/assets/img/testimonial-avata-04.jpg',
                name: 'Mina Hollace',
                role: '/ Freelancer',
            },
        ]
    }),
    mounted() {
        console.log(this.slides);
    }
}
</script>

<template>

    <!-- carousel made with vueperslides -->
    <vueper-slides class="no-shadow" :visibleSlides="3" :slidePerView="1" :draggingDistance="70" :gap="10" :bullets="true">
        <vueper-slide class="slide" v-for="slide in slides" :key="slide" :title="slide.title" :content="slide.content">
        </vueper-slide>
    </vueper-slides>
</template>

<style lang="scss">
@use '../../assets/Styles/AppCarousel.scss'
</style>