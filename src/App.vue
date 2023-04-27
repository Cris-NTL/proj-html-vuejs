<script>
import AppHeader from './components/Header/AppHeader.vue';
import AppMain from './components/main/AppMain.vue';
import Logo from './assets/img/dark-logo.png';

export default{
  components: {
    AppHeader,
    AppMain,
  },

  data() {
    return {
      navItems: {
        logo: { src: Logo, alt: 'logoCompany' },
        links: [
          { name: 'Home', iconClass: 'fas fa-chevron-down' },
          { name: 'Pages', iconClass: 'fas fa-chevron-down' },
          { name: 'Courses', iconClass: 'fas fa-chevron-down' },
          { name: 'Features', iconClass: 'fas fa-chevron-down' },
          { name: 'Blog', iconClass: 'fas fa-chevron-down' },
          { name: 'Shop', iconClass: 'fas fa-chevron-down' },
        ],
        icons: [
          { iconClass: 'far fa-user-circle' },
        ],
        input: { placeholder: ' Search...', iconClass: 'fas fa-search' },
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
