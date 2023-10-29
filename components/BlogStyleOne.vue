<template>
    <section class="blog-area blog-default-area">
        <div class="container">
            <div class="row">
                <div class="col-md-8 col-lg-6 m-auto">
                    <div class="section-title text-center" data-aos="fade-up" data-aos-duration="1000">
                        <h5 class="subtitle line-theme-color">Blog Post</h5>
                        <h2 class="title title-style">Latest News From Givest Blog <img class="img-shape" src="/images/shape/3.png" alt="Image-Givest"></h2>
                    </div>
                </div>
            </div>
            <div class="row mtn-150" data-aos="fade-up" data-aos-duration="1000">
                <div class="col-md-6 col-lg-4 mt-150" v-for="(blog, index) in blogs" :key="index">
                    <div class="post-item">
                        <div class="thumb">
                            <nuxt-link to="/blog-details">
                                <img :src="blog.imgSrc" :alt="blog.title">
                            </nuxt-link>
                            <div class="meta-date">
                                <nuxt-link to="/blog"><span>{{ blog.metaDate }}</span> {{ blog.metaMonth }}</nuxt-link>
                            </div>
                            <div class="shape-line"></div>
                        </div>
                        <div class="content">
                            <div class="inner-content">
                                <div class="meta">
                                    <nuxt-link to="/blog" class="post-category">{{ blog.category }}</nuxt-link>
                                    <div class="post-share">
                                        <button class="icon-share">
                                            <img src="/images/icons/share-line-gradient.png" alt="Icon">
                                        </button>
                                        <ul>
                                            <li v-for="(social, index) in blog.socials" :key="index">
                                                <a :href="social.url" :class="social.addColorClass">
                                                    <i :class="social.icon"></i>
                                                </a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                                <h4 class="title">
                                    <nuxt-link to="/blog-details">{{ blog.title }}</nuxt-link>
                                </h4>
                                <p>{{ blog.desc }}</p>
                            </div>
                            <div class="post-footer">
                                <nuxt-link to="/blog-details" class="btn-theme btn-border-gradient btn-size-xs">
                                    <span>Details <img class="icon icon-img" src="/images/icons/arrow-line-right-gradient.png" alt="Icon"></span>
                                </nuxt-link>
                                <nuxt-link to="/blog" class="post-author">By: Robbins</nuxt-link>
                            </div>
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
                        imgSrc: "/images/blog/1.jpg",
                        metaDate: 26,
                        metaMonth: "January",
                        category: "Celebration",
                        title: "Republic day",
                        desc: "National flag of India is hoisted, patriotic are sung and the national anthem is played. Inmates participate in various activities such as essay writing, painting and cultural performances. ",
                        socials: [
                            {
                                icon: "icofont-facebook",
                                url: "#",
                                addColorClass: "color-facebook"
                            },
                            {
                                icon: "icofont-twitter",
                                url: "#",
                                addColorClass: "color-twitter"
                            },
                            {
                                icon: "icofont-dribbble",
                                url: "#",
                                addColorClass: "color-dribbble"
                            },
                            {
                                icon: "icofont-pinterest",
                                url: "#",
                                addColorClass: "color-pinterest"
                            }
                        ]
                    },
                    {
                        imgSrc: "/images/blog/2.jpg",
                        metaDate: 10,
                        metaMonth: "July",
                        category: "Celebration",
                        title: "Holi",
                        desc: " Holi is celebrated by playing with colours. Inmates sing and dance with joy. Inmates enjoy the holi with making paper craft and other fun activities. Drawing along with delicious food.",
                        socials: [
                            {
                                icon: "icofont-facebook",
                                url: "#",
                                addColorClass: "color-facebook"
                            },
                            {
                                icon: "icofont-twitter",
                                url: "#",
                                addColorClass: "color-twitter"
                            },
                            {
                                icon: "icofont-dribbble",
                                url: "#",
                                addColorClass: "color-dribbble"
                            },
                            {
                                icon: "icofont-pinterest",
                                url: "#",
                                addColorClass: "color-pinterest"
                            }
                        ]
                    },
                    {
                        imgSrc: "/images/blog/3.jpg",
                        metaDate: 15,
                        metaMonth: "August",
                        category: "Celebration",
                        title: "Independence Day",
                        desc: "Our CCI organise various activities to nurture patriotism, including flag hoisting, cultural songs. These activities add fun and are a wonderful way to encourage creativity in inmates.",
                        socials: [
                            {
                                icon: "icofont-facebook",
                                url: "#",
                                addColorClass: "color-facebook"
                            },
                            {
                                icon: "icofont-twitter",
                                url: "#",
                                addColorClass: "color-twitter"
                            },
                            {
                                icon: "icofont-dribbble",
                                url: "#",
                                addColorClass: "color-dribbble"
                            },
                            {
                                icon: "icofont-pinterest",
                                url: "#",
                                addColorClass: "color-pinterest"
                            }
                        ]
                    },
                ]
            }
        },
    };
</script>
