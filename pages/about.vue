<template>
    <div class="main-container">
        <Header />
        <OffCanvasMobileMenu />
        <Breadcrumb items="About us" title="About us" />
        <AboutTwo />
        <!-- <TeamOne /> -->
        <!-- <FunFactOne /> -->
        <div class="mt-100"></div>
        <TestimonialOne />
        <!-- <Sponsor /> -->
        <Footer />
    </div>
</template>

<script>
    export default {
        components: {
            Header: () => import('@/components/Header'),
            OffCanvasMobileMenu: () => import('@/components/OffCanvasMobileMenu'),
            Breadcrumb: () => import('@/components/Breadcrumb'),
            AboutTwo: () => import('@/components/AboutTwo'),
            TeamOne: () => import('@/components/TeamOne'),
            FunFactOne: () => import('@/components/FunFactOne'),
            TestimonialOne: () => import('@/components/TestimonialOne'),
            Sponsor: () => import('@/components/Sponsor'),
            Footer: () => import('@/components/Footer'),
        },
    };
</script>


