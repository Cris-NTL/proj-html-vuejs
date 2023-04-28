<script>
export default {
    name: 'AppFooter',

    props: {
        footerData: {
            type: Object,
            required: true
        }
    },

    methods: {
        scrollToTop() {
            window.scrollTo(0, 0);
        }
    }
}
</script>

<template>
    <section class="footer_section my-5">
        <footer class="footer-dark py-5">
            <div class="container">
                <div class="row">
                    <div class="col-md-6">
                        <h3 class="mb-3 font-weight-bold">{{ footerData.address.title }}</h3>
                        <ul class="list-unstyled">
                            <li class="mb-2" v-for="(detail, index) in footerData.address.details" :key="index">{{ detail }}
                            </li>
                        </ul>
                        <div class="ms_icons d-flex gap-4">
                            <a href="#" class="mr-3" v-for="(icon, index) in footerData.address.icons" :key="index">
                                <i :class="icon.class"></i>
                            </a>
                        </div>
                    </div>
                    <div class="col-md-6 d-flex justify-content-end">
                        <ul class="me-3" v-for="(link, index) in footerData.links" :key="index">
                            <li>
                                <h3 class="mb-3">{{ link.title }}</h3>
                            </li>
                            <li class="mb-2" v-for="(item, idx) in link.items" :key="idx">
                                <a href="#" class="text-decoration-none">{{ item }}</a>
                            </li>
                        </ul>
                    </div>
                    <p class="text-center mt-4">{{ footerData.copyright }}</p>
                </div>
                <button @click="scrollToTop" class="btn"><i class="fa-solid fa-arrow-up-long"></i></button>
            </div>
        </footer>
    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/Styles/AppFooter.scss'
</style>