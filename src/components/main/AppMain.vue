<script>
import AppCourses from './AppCourses.vue';
import AppBenefits from './AppBenefits.vue';
import AppCompanionship from './AppCompanionship.vue';

export default {
    name: 'AppMain',
    
    components: {
        AppCourses,
        AppBenefits,
        AppCompanionship,
    },

}
</script>

<template>
    <main class="container mt-5">
        <AppCourses></AppCourses>
        <AppBenefits></AppBenefits>
        <AppCompanionship></AppCompanionship>
    </main>
</template>

<style lang="scss" scoped>
@use '../../assets/Styles/AppMain.scss'
</style>