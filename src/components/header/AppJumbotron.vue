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
    <section class="jumbo-container container mt-1 d-flex justify-content-evenly py-5">
        <div class="jumbo_text col-lg-4">
            <h1>Distant learning for further expansion</h1>
            <p>Learning is a life-long journey that in fact we never find the terminate stop. Stop searching. Enjoy the
                process.</p>
            <button class="btn btn-primary">Download free guide</button><br>
            <span>Have questions? <span>Get Free Sample</span></span>
        </div>

        <div class="jumbo_img col-lg-8">
            <img src="../../assets/img/about-me-profile-ohm4dxoearqbxny7q3bq1pzbdgofdx0tobbeqcvzd0.jpg" alt="aboutMeAvatar">
        </div>

    </section>

    <AppSponsors></AppSponsors>
</template>

<style lang="scss" scoped>
@use '../../assets/Styles/AppJumbotron.scss'
</style>