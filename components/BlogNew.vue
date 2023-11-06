<template>
    <section class="blog-area blog-default-area">
        <div class="container">
            <div class="row">
                <div class="col-md-8 col-lg-6 m-auto">
                    <div class="section-title text-center" data-aos="fade-up" data-aos-duration="1000">
                        <h5 class="subtitle line-theme-color">Events and Celebrations</h5>
                        <h2 class="title title-style">Latest News From AHSB <img class="img-shape" src="/images/shape/3.png" alt="Image-Givest"></h2>
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
                        metaDate: 26,
                        metaMonth: "January",
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
                    {
                        imgSrc: "/images/events/3.jpeg",
                        metaDate: 15,
                        metaMonth: "August",
                        category: "Celebration",
                        title: "Teachers' day",
                        desc: "Expressing gratitude is at the core of this celebration, with students pouring their hearts into handwritten letters, heartfelt speeches, and handmade cards to convey their thanks. Various competitions are also organised.",
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
                        imgSrc: "/images/events/7.jpeg",
                        metaDate: 21,
                        metaMonth: "February",
                        category: "Celebration",
                        title: "Foundation day",
                        desc: "On 21 February, we celebrate our foundation day, along with the death anniversary of Acharya H. Das. Eminent personalities were invited to encourage inmates to follow footprints of A. H. Das and several events were conducted.",
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
                        imgSrc: "/images/events/6.jpeg",
                        metaDate: 5,
                        metaMonth: "June",
                        category: "Celebration",
                        title: "World Environment Day",
                        desc: "Different activities like massive cleaning drive, plantation etc arranged inside and outside the campus by engaging inmates in the effort to protect the environment. ",
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
                        imgSrc: "/images/events/9.jpeg",
                        metaDate: 15,
                        metaMonth: "August",
                        category: "Celebration",
                        title: "Saraswati Puja ",
                        desc: "Our inmates celebrated the festival by wearing new clothes on the day before puja. The inmates offer “Puspanjali“ at the feet of the goddess gives her blessing. After puja they sit together and enjoy the Sweet Prasad.",
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
                    },{
                        imgSrc: "/images/events/5.jpeg",
                        metaDate: 15,
                        metaMonth: "August",
                        category: "Celebration",
                        title: "Holi",
                        desc: "Holi is celebrated by playing with colours. All our inmates look forward to this festival. Inmates sing and dance with joy. Inmates enjoy the holi with making paper craft, drawing along with delicious food.",
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
                        imgSrc: "/images/events/8.jpeg",
                        metaDate: 14,
                        metaMonth: "November",
                        category: "Celebration",
                        title: "Children's Day",
                        desc: " We organise several events such as debate, painting, solo song, debate etc to develop the inherent potential amongst them. Children enthusiastically participate and  inculcate the ideology of Pandit Jawahar Lal Neheru ",
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
                        imgSrc: "/images/events/11.jpeg",
                        metaDate: 26,
                        metaMonth: "January",
                        category: "Celebration",
                        title: "Republic day",
                        desc: "National flag of India is hoisted, patriotic are sung and the national anthem is played. Inmates participate in various activities such as essay writing,  painting and cultural performances. Prizes were also given to best performers.",
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
                        imgSrc: "/images/events/11.jpeg",
                        metaDate: 15,
                        metaMonth: "August",
                        category: "Celebration",
                        title: "Independence  day",
                        desc: "Our CCI organise various activities to nurture patriotism, including flag hoisting, cultural songs. These activities encourage inmates to nurture their creativity and inform about the sacrifices of our brave leaders.",
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
                        imgSrc: "/images/events/10.jpg",
                        metaDate: 15,
                        metaMonth: "August",
                        category: "Celebration",
                        title: "Ganesh Puja",
                        desc: "Our inmates celebrated the festival by wearing new clothes on the day before puja. The inmates offer “Puspanjali“ at the feet of the goddess gives her blessing. After puja they sit together and enjoy the Sweet Prasad.",
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
