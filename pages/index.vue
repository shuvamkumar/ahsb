<template>
    <div class="home-default-wrapper">
        <Header />
        <OffCanvasMobileMenu />
        <HeroOne />
        <AboutOne />
        <ServiceOne />
        <CausesOne />
        <!-- <DonationStyleOne /> -->
        <!-- <FunFactOne /> -->
        <!-- <EventsOne /> -->
        <TestimonialOne />
        <BlogStyleOne />
        <Footer />
    </div>
</template>

<script>
    export default {
        components: {
            Header: () => import('@/components/Header'),
            OffCanvasMobileMenu: () => import('@/components/OffCanvasMobileMenu'),
            HeroOne: () => import('@/components/HeroOne'),
            AboutOne: () => import('@/components/AboutOne'),
            ServiceOne: () => import('@/components/ServiceOne'),
            CausesOne: () => import('@/components/CausesOne'),
            DonationStyleOne: () => import('@/components/DonationStyleOne'),
            FunFactOne: () => import('@/components/FunFactOne'),
            EventsOne: () => import('@/components/EventsOne'),
            TestimonialOne: () => import('@/components/TestimonialOne'),
            BlogStyleOne: () => import('@/components/BlogStyleOne'),
            Footer: () => import('@/components/Footer'),
        },
    };
</script>


