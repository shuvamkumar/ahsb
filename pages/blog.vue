<template>
    <div class="blog-page-wrapper">
        <Header />
        <OffCanvasMobileMenu />
        <Breadcrumb items="Events" title="All events and celebrations" />
        <!-- <BlogGridWrapper /> -->
        <BlogNew />
        <Footer />
    </div>
</template>

<script>
    export default {
        components: {
            Header: () => import('@/components/Header'),
            OffCanvasMobileMenu: () => import('@/components/OffCanvasMobileMenu'),
            Breadcrumb: () => import('@/components/Breadcrumb'),
            BlogGridWrapper: () => import('@/components/BlogGridWrapper'),
            Footer: () => import('@/components/Footer'),
        }
    };
</script>


