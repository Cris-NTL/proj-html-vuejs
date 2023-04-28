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

    <!-- benefits section -->
    <section class="benefits_section d-flex flex-column pb-5">
        
        <!-- title + subtitle -->
        <div class="text-center mb-5 pt-5">
            <h6>MAXCOACH AVAILABLE COURSES</h6>
            <h3 class="fw-bold my-3">Access
                <span class="fw-normal">
                    Smart Tutoring
                </span>
                Program For Benefits.
            </h3>
        </div>

        <!-- card + image -->
        <div class="container px-5">
            <div class="row d-flex flex-wrap">
                <div class="col-12 col-md-4 mb-5" v-for="(image, index) in benefitImages" :key="index">
                    <div class="d-flex flex-column align-items-center">
                        <div class="img_container mb-3">
                            <img :src="image" alt="course">
                        </div>

                        <!-- details -->
                        <div class="benefits_details">
                            <h5 class="fw-bold">Customize Preference</h5>
                            <p>Learners are given the right to arrange and customize their study schedule and timetable based on preferences.</p>
                            <a class="fw-bold" href="#">Start here <i class="fa-solid fa-right-long"></i></a>
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