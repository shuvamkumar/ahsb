<template>
    <div class="donners-info">
        <h3>Great Donners</h3>
        <div class="donners-item">
            <div class="donner-item" v-for="(donner, index) in donnerList" :key="index">
                <img :src="donner.imgSrc" :alt="donner.alt">
            </div>
            <div class="donner-item donner-number">+286</div>
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                donnerList: [
                    {
                        imgSrc: "",
                        alt: "image"
                    },
                    {
                        imgSrc: "",
                        alt: "image"
                    },
                    {
                        imgSrc: "",
                        alt: "image"
                    },
                    {
                        imgSrc: "",
                        alt: "image"
                    },
                    {
                        imgSrc: "",
                        alt: "image"
                    },
                    {
                        imgSrc: "",
                        alt: "image"
                    },
                    {
                        imgSrc: "",
                        alt: "image"
                    },
                    {
                        imgSrc: "",
                        alt: "image"
                    },
                    {
                        imgSrc: "",
                        alt: "image"
                    },
                    {
                        imgSrc: "",
                        alt: "image"
                    },
                    {
                        imgSrc: "",
                        alt: "image"
                    },
                    {
                        imgSrc: "",
                        alt: "image"
                    },
                    {
                        imgSrc: "",
                        alt: "image"
                    },
                ]
            }
        },
    };
</script>