<script>
import AppSponsors from './AppSponsors.vue';

export default {
    name: 'AppJumbotron',

    components: {
        AppSponsors,
    }
}
</script>

<template>
    
    <!-- jumbotron container -->
    <section class="jumbo-container d-flex justify-content-evenly py-5">
        
        <!-- details -->
        <div class="jumbo_text col-lg-4">
            <h1>Distant learning for further expansion</h1>
            <p>Learning is a life-long journey that in fact we never find the terminate stop. Stop searching. Enjoy the
                process.</p>
            <button class="btn mb-3 px-4 fw-bold">
                <i class="fa-solid fa-download px-2"></i>
                Download free guide
            </button><br>
            <span class="link_question fw-bold">Have questions?
                <span class="link_download">Get Free Sample
                    <i class="fa-solid fa-right-long"></i>
                </span>
            </span>
        </div>

        <!-- avatar + images -->
        <div class="jumbo_img col-lg-8">
            <img class="avatar" src="../../assets/img/about-me-profile-ohm4dxoearqbxny7q3bq1pzbdgofdx0tobbeqcvzd0.jpg" alt="aboutMeAvatar">
            <img class="secondary_img" src="../../assets/img/maxcoach-shape-02.png" alt="secondaryImage">
            <img class="tirtiary_img" src="../../assets/img/maxcoach-shape-07.png" alt="tertiaryImage">
            <img class="quaternary_img my-2" src="../../assets/img/maxcoach-shape-07-100x100.png" alt="quaternaryImage">
            <img class="quinary_img my-2" src="../../assets/img/maxcoach-shape-07-100x100.png" alt="quinaryImage">
            <div class="ms_ring"></div>
        </div>

    </section>

    <!-- sponsors component -->
    <AppSponsors></AppSponsors>
</template>

<style lang="scss" scoped>
@use '../../assets/Styles/AppJumbotron.scss'
</style>