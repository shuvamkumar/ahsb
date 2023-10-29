<template>
    <section class="testimonial-area testimonial-default-area bgcolor-theme3 position-relative">
        <div class="container">
            <div class="row">
                <div class="col-md-12 col-lg-4 col-xl-5 position-static">
                    <div class="title-wrp" :style="{ backgroundImage: `url('/images/testimonial/bg-testi1.jpg')` }">
                        <div class="section-title">
                            <h5 class="subtitle line-white-color text-white mb-7">Recent Events</h5>
                            <h2 class="title title-style text-white">
                                What People Say About Us. 
                                <img class="img-shape" src="/images/shape/3.png" alt="Image-Givest">
                            </h2>
                        </div>
                    </div>
                </div>
                <div class="col-md-12 col-lg-7 col-xl-6 position-static">
                    <div class="testimonial-content">
                        <div class="testimonial-slider-content">
                            <div class="testimonial-slider-container">
                                <swiper
                                    :speed="1000"
                                    :loop="true"
                                    :navigation="swiperOptions.navigation"
                                >
                                    <swiper-slide class="testimonial-single" v-for="(testimonial, index) in testimonials" :key="index">
                                        <!-- <div class="client-thumb-wrp">
                                            <div class="client-thumb">
                                                <img :src="testimonial.imgSrc" :alt="testimonial.name">
                                            </div>
                                            <div class="quote-icon">“</div>
                                        </div> -->
                                        <div class="client-content">
                                            <p>{{ testimonial.desc }}</p>
                                        </div>
                                        <div class="client-info">
                                            <img class="shape-line-img" src="/images/shape/line-t1.png" alt="Image-Givest">
                                            <h4 class="name">{{ testimonial.name }}</h4>
                                            <!-- <h6 class="designation">{{ testimonial.designation }}</h6> -->
                                        </div>
                                    </swiper-slide>
                                </swiper>
                                <!-- Add Arrows -->
                                <div class="navigation-wrp">
                                    <div class="swiper-button-prev">
                                        <img class="icon-img" src="/images/icons/test-arrow-left.png" alt="Image-Icon">
                                    </div>
                                    <div class="swiper-button-next">
                                        <img class="icon-img" src="/images/icons/test-arrow-right.png" alt="Image-Icon">
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    import { Swiper, SwiperSlide } from "swiper/vue"
    import { ref } from 'vue'
    import SwiperCore, { Navigation } from 'swiper/core'
    SwiperCore.use([Navigation ])

    import "swiper/css"
    const count = ref(0)

    export default {
        components: {
            Swiper,
            SwiperSlide
        },
        data() {
            return {
                swiperOptions: {
                    navigation: {
                        nextEl: '.swiper-button-next',
                        prevEl: '.swiper-button-prev',
                    },
                },

                testimonials: [
                    {
                        imgSrc: "/images/testimonial/1.png",
                        desc: "The origin, relevant development, acknowledging contributors, replication of action-learning that manifest further qualitative service for deprived poor (disadvantaged children) have added value to our effort to expand operational periphery and taking up much more issue based pro-poor initiatives eventually integrated to organization’s relevant endeavors.",
                        name: "Hon'ble Secretary",
                        designation: "Senior Volunteer"
                    },
                    {
                        imgSrc: "/images/testimonial/2.png",
                        desc: "Acharya Harihar Sishu Bhawan is not at all a large and complex organization. But it is always bent upon to build a professional attitude & approach to development. The management, till now has set professional standards of attitude & fitness for work which is characterized by responsiveness & quality consciousness. And this is the main aptitude that will one day enable the organization as one of the successful organizations in protection and promotion of disadvantaged children both at rural and urban level – focusing on all districts of Orissa",
                        name: "Hon'ble President",
                        designation: "Junior Volunteer"
                    },
                    {
                        imgSrc: "/images/testimonial/2.png",
                        desc: "From our long association with innocent disadvantaged children and our personal throb towards the deprived people we hold that – Disadvantage and Deprivation, regardless of age  and gender. With this understanding, we started this venture not as a mere centre for rescue but as a Voluntary Development Organization. And in fact, we do realize our social commitment and responsibility very well",
                        name: "Hon'ble Vice-President",
                        designation: "Junior Volunteer"
                    },
                    {
                        imgSrc: "/images/testimonial/2.png",
                        desc: "Developing leadership within the downtrodden, empowering them to have confiddence upon themselves & helping them maintain their life and livelihood have been the prime concern of Acharya Harihar Sishu Bhawan since its very inception in the underdeveloped pocket of a develped district of Odisha. Emergence of new situations in these years has posed major challenges before the people & organization as well. ",
                        name: "Smt.Rajalaxmi Dash, Leading woman member of executive body",
                        designation: "Junior Volunteer"
                    }
                ]
            }
        },
    };
</script>
