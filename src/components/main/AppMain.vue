<script>
import AppCourses from './AppCourses.vue';
import AppBenefits from './AppBenefits.vue';
import AppCompanionship from './AppCompanionship.vue';
import AppLearners from './AppLearners.vue';

export default {
    name: 'AppMain',
    
    components: {
        AppCourses,
        AppBenefits,
        AppCompanionship,
        AppLearners,
    },

}
</script>

<template>
    <main class= "mt-5">
        <AppCourses></AppCourses>
        <AppBenefits></AppBenefits>
        <AppCompanionship></AppCompanionship>
        <AppLearners></AppLearners>
    </main>
</template>

<style lang="scss" scoped>
@use '../../assets/Styles/AppMain.scss'
</style>