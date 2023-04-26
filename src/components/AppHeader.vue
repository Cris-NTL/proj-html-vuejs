<script>
import AppJumbotron from './AppJumbotron.vue';

export default {
    components: {
        AppJumbotron,
    },

    props: {
        navItems: {
            type: Object,
            required: true,
        },
    },
};
</script>

<template>
    <!-- header section -->
    <header class="header_container container d-flex align-items-center">
        <nav class="d-flex align-items-center">
            <div class="col-lg-2">
                <img :src="navItems.logo.src" alt="logoCompany">
            </div>

            <!-- links + search input -->
            <ul class="d-flex col-lg-10 justify-content-lg-end gap-3 m-0">
                <li v-for="link in navItems.links" :key="link.name">
                    {{ link.name }}
                </li>
                <li v-for="icon in navItems.icons" :key="icon.iconClass">
                    <i :class="icon.iconClass"></i>
                </li>
                <li>
                    <input :placeholder="navItems.input.placeholder" type="text">
                </li>
            </ul>
        </nav>
    </header>

    <!-- jumbotron section -->
    <AppJumbotron></AppJumbotron>
</template>

<style lang="scss">
@use '../assets/Styles/AppHeader.scss';
</style>
