<template>
    <div class="container mx-auto py-12">
        <div>
            <h1 class="text-center text-4xl font-semibold">Our Blog</h1>
            <div class="py-8 md:grid grid-cols-3 px-4 gap-6">
                <div v-for="(blog, index) in blogs" :key="index">
                     <img :src="blog.image" alt="">
                    <p class="text-sm py-3">{{ blog.date }}</p>
                    <h1 class="text-xl font-semibold">{{ blog.title }}</h1>
                    <p class="text-sm py-4">{{ blog.description }}</p>
                    <div class="flex gap-1 hover:text-[#2405F2]">
                        <button>Read More</button>
                        <svg class="my-2" width="25" height="12" viewBox="0 0 25 12" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M24.5303 6.53033C24.8232 6.23744 24.8232 5.76256 24.5303 5.46967L19.7574 0.696699C19.4645 0.403806 18.9896 0.403806 18.6967 0.696699C18.4038 0.989593 18.4038 1.46447 18.6967 1.75736L22.9393 6L18.6967 10.2426C18.4038 10.5355 18.4038 11.0104 18.6967 11.3033C18.9896 11.5962 19.4645 11.5962 19.7574 11.3033L24.5303 6.53033ZM0 6.75H24V5.25H0V6.75Z" fill="#282938"/>
                        </svg>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
const blogs = [
    {
        image: '/img/blog1.png',
        date: '27 Jan 2021',
        title: 'How one Webflow user grew his single person consultancy from $0-100K in 14 months',
        description: 'See how pivoting to Webflow changed one person’s sales strategy and allowed him to attract'
    },
    {
        image: '/img/blog2.png',
        date: '27 Jan 2021',
        title: 'How one Webflow user grew his single person consultancy from $0-100K in 14 months',
        description: 'See how pivoting to Webflow changed one person’s sales strategy and allowed him to attract'
    },
    {
        image: '/img/blog3.png',
        date: '27 Jan 2021',
        title: 'How one Webflow user grew his single person consultancy from $0-100K in 14 months',
        description: 'See how pivoting to Webflow changed one person’s sales strategy and allowed him to attract'
    },
    {
        image: '/img/blog4.png',
        date: '27 Jan 2021',
        title: 'How one Webflow user grew his single person consultancy from $0-100K in 14 months',
        description: 'See how pivoting to Webflow changed one person’s sales strategy and allowed him to attract'
    },
    {
        image: '/img/blog5.png',
        date: '27 Jan 2021',
        title: 'How one Webflow user grew his single person consultancy from $0-100K in 14 months',
        description: 'See how pivoting to Webflow changed one person’s sales strategy and allowed him to attract'
    },
    {
        image: '/img/blog6.png',
        date: '27 Jan 2021',
        title: 'How one Webflow user grew his single person consultancy from $0-100K in 14 months',
        description: 'See how pivoting to Webflow changed one person’s sales strategy and allowed him to attract'
    }
];
</script>

<style scoped>

</style>
