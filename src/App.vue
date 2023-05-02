<script>
import AppHeader from './components/header/AppHeader.vue';
import AppMain from './components/main/AppMain.vue';
import AppFooter from './components/footer/AppFooter.vue';
import Logo from './assets/img/dark-logo.png';

export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter,
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

      footerData: {
        address: {
          title: 'Address',
          details: [
            '382 NE 191st ST # 87394 Miami, FL 33179-3899',
            '+1(305) 547-9909 (9am - 5pm EST, Monday - Friday)',
            'support@maxcoach.com'
          ],
          icons: [
            { href: '#', class: 'fa-brands fa-facebook fa-bounce fa-2xl' },
            { href: '#', class: 'fa-brands fa-twitter fa-bounce fa-2xl' },
            { href: '#', class: 'fa-brands fa-square-instagram fa-bounce fa-2xl' },
            { href: '#', class: 'fa-brands fa-linkedin fa-bounce fa-2xl' }
          ]
        },
        links: [
          {
            title: 'Explore',
            items: ['Start here', 'Blog', 'About us']
          },
          {
            title: '---',
            items: ['Success story', 'Courses', 'Contact us']
          },
          {
            title: 'Information',
            items: ['Merchandising', 'Purchase guide', 'Privacy policy', 'Terms of services']
          }
        ],
        copyright: '© 2020 Maxcoach. All Rights Reserved'
      }

    };
  },
};
</script>

<template>
  <AppHeader :navItems="navItems"></AppHeader>
  <AppMain></AppMain>
  <AppFooter :footerData="footerData"></AppFooter>
</template>

<style lang="scss">
@use './assets/styles/general.scss';
</style>
