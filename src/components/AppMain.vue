<script>
import AppCourses from './AppCourses.vue';
import AppBenefits from './AppBenefits.vue';

export default {
    name: 'AppMain',
    
    components: {
        AppCourses,
        AppBenefits,
    },

}
</script>

<template>
    <main class="container mt-5">
        <AppCourses></AppCourses>
        <AppBenefits></AppBenefits>
    </main>
</template>

<style lang="scss" scoped>
@use '../assets/Styles/AppMain.scss'
</style>