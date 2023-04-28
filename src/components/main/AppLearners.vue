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
    <section class="learners_section d-flex flex-column py-5">

        <div class="text-center mb-5 pt-5">
            <h6>GREAT WORDS ABOUT MAXCOACH</h6>
            <h3 class="fw-bold my-3">
                Our
                <span class="fw-normal">
                    top learners'
                </span>
                verbatim
            </h3>
        </div>

        <AppCarousel></AppCarousel>
    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/Styles/AppLearners.scss'
</style>