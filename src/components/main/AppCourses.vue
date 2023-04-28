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

    <!-- courses section -->
    <section class="courses_section container">
        
        <!-- title + subtitle -->
        <div class="text-center my-5">
            <h6>STIMULATED TO LEARN?</h6>
            <h3 class="fw-bold">Featured Online Courses</h3>
        </div>

        <!-- grid with cards -->
        <div class="container">
            <div class="row d-flex flex-wrap">
                <div class="col-12 col-md-6 mb-5" v-for="col in 6" :key="col">
                    <div class="d-flex justify-content-center">
                        <div class="img_container">
                            <img :src="courseImages[col - 1]" alt="course">
                        </div>
                        <div class="course_details d-flex flex-wrap flex-column justify-content-lg-center mx-3">
                            <h5 class="fw-bold">Free</h5>
                            <h6 class="fw-bold">Learning to Write as a Professional Author</h6>
                            <span>
                                <i class="fa-regular fa-file me-1"></i>
                                20 lessons
                                <span>
                                    <i class="fa-regular fa-user mx-1"></i>
                                    50 students
                                </span>
                            </span>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- download button -->
        <div class="text-center mb-5">
            <button class="btn px-5 my-4 fw-bold">
                View all courses
                <i class="fa-solid fa-right-long"></i>
            </button>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/Styles/AppCourses.scss'
</style>