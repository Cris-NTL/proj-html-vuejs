<script>
import AppJumbotron from './AppJumbotron.vue';

export default {
    name: 'AppHeader',
    
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
    <header class="header_container d-flex align-items-center justify-content-center">
        <nav class="d-flex align-items-center">
            <div class="col-lg-2">
                <img :src="navItems.logo.src" alt="logoCompany">
            </div>

            <!-- links + search input -->
            <ul class="d-flex col-lg-10 justify-content-lg-end gap-3 m-0 align-items-center">
                <li class="d-flex align-items-center" v-for="link in navItems.links" :key="link.name">
                    {{ link.name }}
                    <i class="chevron_arrow mx-1" :class="link.iconClass"></i>
                </li>
                <li v-for="icon in navItems.icons" :key="icon.iconClass">
                    <i :class="icon.iconClass"></i>
                </li>
                <li>
                    <input class="border-0 p-1 rounded-pill" :placeholder="navItems.input.placeholder" type="text">
                    <i class="mx-2" :class="navItems.input.iconClass"></i>
                </li>
            </ul>
        </nav>
    </header>

    <!-- jumbotron section -->
    <AppJumbotron></AppJumbotron>
</template>

<style lang="scss">
@use '../../assets/Styles/AppHeader.scss';
</style>
