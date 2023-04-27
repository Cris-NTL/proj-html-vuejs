<script>
export default {
    name: 'AppCourses',

    data() {
        return {
            courseImages: [
                '/src/assets/img/course-02-480x298.jpg',
                '/src/assets/img/stock-full-hd-03-480x298.jpg',
                '/src/assets/img/stock-full-hd-04-480x298.jpg',
                '/src/assets/img/stock-full-hd-06-480x298.jpg',
                '/src/assets/img/course-featured-image-01-480x298.jpg',
                '/src/assets/img/stock-full-hd-05-480x298.jpg',
            ],
        };
    },
};
</script>

<template>
    <div class="text-center my-5">
        <h6>stimulated to learn?</h6>
        <h3>Featured Online Courses</h3>
    </div>

    <div class="container px-5">
        <div class="row d-flex flex-wrap">
            <div class="col-12 col-md-6 mb-5" v-for="col in 6" :key="col">
                <div class="d-flex justify-content-center">
                    <div class="img_container">
                        <img :src="courseImages[col - 1]" alt="course">
                    </div>
                    <div class="d-flex flex-wrap flex-column justify-content-lg-center mx-3">
                        <h5>Free</h5>
                        <h6>Learning to Write as a Professional Author</h6>
                        <span>20 lessons</span><span>50 students</span>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <div class="text-center mb-5">
        <button class="btn btn-primary">View all courses -></button>
    </div>
</template>

<style lang="scss" scoped>
@use '../../assets/Styles/AppCourses.scss'
</style>