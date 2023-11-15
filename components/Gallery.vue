<template>
    <section class="blog-area blog-default-area">
        <div class="container">
            <div class="row mtn-150" data-aos="fade-up" data-aos-duration="1000">
                <div class="col-md-6 col-lg-4 mt-60" v-for="(blog, index) in blogs" :key="index">
                    <div class="post-item">
                        <div class="thumb">
                            <nuxt-link to="#">
                                <img :src="blog.imgSrc" :alt="blog.title">
                            </nuxt-link>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        data() {
            return {
                blogs: [
                    {
                        imgSrc: "/images/events/1.jpeg",
                    },
                    {
                        imgSrc: "/images/events/2.jpeg",
                    },
                    {
                        imgSrc: "/images/events/3.jpeg",
                    },
                    {
                        imgSrc: "/images/events/4.jpg",
                    },
                    {
                        imgSrc: "/images/events/5.jpeg",
                    },
                    {
                        imgSrc: "/images/events/6.jpeg",
                    },
                    {
                        imgSrc: "/images/events/7.jpeg",
                    },
                    {
                        imgSrc: "/images/events/8.jpeg",
                    },
                    {
                        imgSrc: "/images/events/9.jpeg",
                    },
                    {
                        imgSrc: "/images/events/10.jpg",
                    },
                    {
                        imgSrc: "/images/events/11.jpeg",
                    },
                    {
                        imgSrc: "/images/events/12.jpeg",
                    },
                    {
                        imgSrc: "/images/events/13.jpeg",
                    },
                    {
                        imgSrc: "/images/events/14.jpeg",
                    },
                    {
                        imgSrc: "/images/events/15.jpeg",
                    },
                    // {
                    //     imgSrc: "/images/events/16.jpeg",
                    // },
                    {
                        imgSrc: "/images/events/17.jpeg",
                    },
                    {
                        imgSrc: "/images/events/18.jpeg",
                    },
                    {
                        imgSrc: "/images/events/19.jpeg",
                    },
                    {
                        imgSrc: "/images/events/20.jpeg",
                    },
                    {
                        imgSrc: "/images/events/21.jpeg",
                    },
                    {
                        imgSrc: "/images/events/22.jpeg",
                    },
                    // {
                    //     imgSrc: "/images/events/23.jpeg",
                    // },
                ]
            }
        },
    };
</script>
