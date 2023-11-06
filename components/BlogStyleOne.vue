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
                                    <!-- <div class="post-share">
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
                                    </div> -->
                                </div>
                                <h4 class="title">
                                    <nuxt-link to="/blog-details">{{ blog.title }}</nuxt-link>
                                </h4>
                                <p>{{ blog.desc }}</p>
                            </div>
                            <div class="post-footer">
                                <!-- <nuxt-link to="/blog-details" class="btn-theme btn-border-gradient btn-size-xs">
                                    <span>Details <img class="icon icon-img" src="/images/icons/arrow-line-right-gradient.png" alt="Icon"></span>
                                </nuxt-link> -->
                                <nuxt-link to="/blog" class="post-author">By: Pratyush</nuxt-link>
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
                        imgSrc: "/images/events/4.jpg",
                        metaDate: 2,
                        metaMonth: "October",
                        category: "Celebration",
                        title: "Gandhi Jayanti",
                        desc: "On the occasion of Gandhi Jayanti, multiple events like quiz contests, speech and song competition are organised. Inmates are taught of the values and practices imparted by Gandhi ji. A small cleanliness campaign is also held.",
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
                        imgSrc: "/images/events/2.jpeg",
                        metaDate: 10,
                        metaMonth: "July",
                        category: "Celebration",
                        title: "Mahak 'n' Utschah",
                        desc: "District and state level events are organised as mahak and utschah to create a child friendly atmosphere. Inmates participated in cultural and athletic events,  allowing them to explore their interests and abilities.",
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
                        imgSrc: "/images/events/1.jpeg",
                        metaDate: 15,
                        metaMonth: "August",
                        category: "Celebration",
                        title: "Rakhsa Bandhan",
                        desc: "Celebrating Raksha Bandhan, the staffs of AHSB tied the sacred thread to inmates and expressed their gratitude for their Raksha with the bandhan. This is a symbol of universal brotherhood and to foster the spirit of love.",
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
