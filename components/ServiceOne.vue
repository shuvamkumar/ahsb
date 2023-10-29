<template>
    <section class="service-area service-default-area">
        <div class="container">
            <div class="row mtn-30" data-aos="fade-up" data-aos-duration="1000">
                <div class="col-md-6 col-lg-4 mt-30" v-for="(service, index) in services" :key="index">
                    <div class="icon-box-item box-height" :class="service.addClassName">
                        <div class="icon-box-top">
                            <div class="icon-box">
                                <img class="icon-img" :src="service.icon" alt="icon" />
                            </div>
                            <h4 class="title">{{ service.title }}</h4>
                        </div>
                        <div class="content">
                            <div class="separator-line">
                                <img src="/images/shape/line-s1.png" alt="shape" />
                            </div>
                            <p>{{ service.desc }}</p>
                            
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
                services: [
                    {
                        icon: "/images/icons/s1.png",
                        title: "Vision",
                        desc: "To show path to all deprived people of society which is just and participatory, free from all sorts of discrimination ensuring equal rights to all irrespective of Caste, Creed, Sex and Religion ",
                        addClassName: "item-one"
                    },
                    {
                        icon: "/images/icons/s2.png",
                        title: "Mission",
                        desc: "To empower the poor mass, develop their potential, improve their socio-economic status and eradiate poverty thereby bringing sustainable development with emphasis on weaker and vulnerable section.",
                        addClassName: "item-two"
                    },
                    {
                        icon: "/images/icons/s3.png",
                        title: "Objective",
                        desc: "To work for forming a society free from any discrimination ensuring possibilities of all possible support to neglected mass, esp. the vulnerable through capacitation & development.",
                        addClassName: "item-three"
                    }
                ]
            }
        },
    };
</script>
