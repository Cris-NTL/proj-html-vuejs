<script>
export default {
    name: 'AppBenefits',

    data() {
        return {
            benefitImages: [
                '/src/assets/img/home-2-image-box-01.png',
                '/src/assets/img/about-us-02-image-box-02.png',
                '/src/assets/img/home-2-image-box-03.png',
            ],
        };
    },
};
</script>

<template>
    <section class="benefits_section d-flex flex-column">
        <div class="text-center mb-5 pt-5">
            <h6>MaxCoach Available Courses</h6>
            <h3>Access <span>Smart Tutoring</span> Program For Benefits.</h3>
        </div>

        <div class="container px-5">
            <div class="row d-flex flex-wrap">
                <div class="col-12 col-md-4 mb-5" v-for="(image, index) in benefitImages" :key="index">
                    <div class="d-flex flex-column align-items-center">
                        <div class="img_container mb-3">
                            <img :src="image" alt="course">
                        </div>
                        <div>
                            <h5>Customize Preference</h5>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde at perspiciatis aut, adipisci
                                ad a
                                odit beatae nulla? Est, ipsa.</p>
                            <a href="#">Start here -></a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/Styles/AppBenefits.scss'
</style>