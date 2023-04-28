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
                img: '@/assets/img/testimonial-avata-02.jpg',
                name: 'Mina Hollace',
                role: '/ Freelancer',
            },
            {
                title: 'High level of efficiency and scientific teaching methods',
                content: 'I am free to learn at my own pace, follow my own schedule and choose the subject i want to learn from the syllabus. Great study portal fro people like me.',
                img: '@/assets/img/testimonial-avata-02.jpg',
                name: 'Mina Hollace',
                role: '/ Freelancer',
            },
            {
                title: 'High level of efficiency and scientific teaching methods',
                content: 'I am free to learn at my own pace, follow my own schedule and choose the subject i want to learn from the syllabus. Great study portal fro people like me.',
                img: '@/assets/img/testimonial-avata-02.jpg',
                name: 'Mina Hollace',
                role: '/ Freelancer',
            },
            {
                title: 'High level of efficiency and scientific teaching methods',
                content: 'I am free to learn at my own pace, follow my own schedule and choose the subject i want to learn from the syllabus. Great study portal fro people like me.',
                img: '@/assets/img/testimonial-avata-02.jpg',
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
    <vueper-slides class="no-shadow" :visibleSlides="3" :slidePerView="1" :draggingDistance="70" :gap="10" :bullets="false">
        <vueper-slide class="slide" v-for="slide in slides" :key="slide.title">
            <div class="slide-content">
                <h5>{{ slide.title }}</h5>
                <p>{{ slide.content }}</p>
                <div class="slide-footer">
                    <img class="profile-image" :src="slide.img" :alt="slide.name">
                    <div>
                        <h6>{{ slide.name }}</h6>
                        <span>{{ slide.role }}</span>
                    </div>
                </div>
            </div>
        </vueper-slide>
    </vueper-slides>
</template>

<style lang="scss">
@use '../../assets/Styles/AppCarousel.scss'
</style>