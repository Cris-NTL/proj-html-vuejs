<script>
import AppHeader from './components/header/AppHeader.vue';
import AppMain from './components/main/AppMain.vue';
import Logo from './assets/img/dark-logo.png';

export default {
  components: {
    AppHeader,
    AppMain,
  },

  data() {
    return {
      navItems: {
        logo: { src: Logo, alt: 'logoCompany' },
        links: [
          { name: 'Home' },
          { name: 'Pages' },
          { name: 'Courses' },
          { name: 'Features' },
          { name: 'Blog' },
          { name: 'Shop' },
        ],
        icons: [
          { iconClass: 'bi bi-person' },
        ],
        input: { placeholder: 'Search...' },
      },
    };
  },
};
</script>

<template>
  <AppHeader :navItems="navItems"></AppHeader>
  <AppMain></AppMain>
</template>

<style lang="scss">
@use './assets/styles/general.scss';
</style>
