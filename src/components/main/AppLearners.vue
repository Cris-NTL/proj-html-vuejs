<script>
import AppCarousel from './AppCarousel.vue';

export default {
    name: 'AppLearners',

    components: {
        AppCarousel,
    }

}
</script>

<template>

    <!-- learners section -->
    <section class="learners_section d-flex flex-column py-5">

        <!-- title + subtitle -->
        <div class="text-center pt-5">
            <h6>GREAT WORDS ABOUT MAXCOACH</h6>
            <h3 class="fw-bold my-3">
                Our
                <span class="fw-normal">
                    top learners'
                </span>
                verbatim
            </h3>
        </div>

        <!-- carousel component -->
        <AppCarousel></AppCarousel>
        
        
    </section>

    <!-- get started section -->
    <section class="ms_started d-flex justify-content-center mt-5">
        <div class="wrapper text-center">
            <img class="secondary_img" src="../../assets/img/maxcoach-shape-01.png" alt="secondaryImage">
            <div class="ms_ring"></div>
            <img class="tertiary_img" src="../../assets/img/maxcoach-shape-02.png" alt="tertiaryImage">
            <h5>Start today for getting <span>Online Certification</span></h5>
            <h3 class="mb-4">You can be your own guiding star wirh our help!</h3>
            <button class="btn">Get started now</button>
        </div>
    </section>

</template>

<style lang="scss" scoped>
@use '../../assets/Styles/AppLearners.scss'
</style>