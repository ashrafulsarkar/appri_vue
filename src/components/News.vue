<script setup>
const posts = [
    {
        title: 'Sitting proudly atop M3565 is the two-storey penthouse',
        author: 'Admin',
        date: '11 Dec 2023',
        img: '/img/news/news1.png'
    },
    {
        title: 'Technology are the two-storey pen tho use with gor geous',
        author: 'Admin',
        date: '11 Dec 2023',
        img: '/img/news/news2.png'
    },
    {
        title: 'Sitting proudly atop M3565 is the two-storey penthouse',
        author: 'Admin',
        date: '11 Dec 2023',
        img: '/img/news/news3.png'
    },
]
</script>
<template>
    <!-- news area start -->
    <section id="news" class="news-area pt-60 pb-125">
        <div class="container">
            <div class="row">
                <div class="col-xl-12">
                    <div class="section-title text-center pb-55">
                        <h2>Latest News</h2>
                        <p>Enables you to define cross-channel profiles and improve audience. sessions per week</p>
                    </div>
                </div>
            </div>
            <div class="row">
                <div class="col-xl-4 col-lg-4 col-md-4" v-for="post in posts">
                    <div class="news-blog mb-30">
                        <div class="news-img">
                            <img :src="post.img" :alt="post.title">
                        </div>
                        <div class="news-text">
                            <div class="news-info">
                                <div class="news-info-item f-left"><i class="fas fa-calendar-alt"></i>{{ post.date }}</div>
                                <div class="news-info-item f-right"><i class="fas fa-user"></i>{{ post.author }}</div>
                            </div>
                            <div class="news-title">
                                <h4>{{ post.title }}</h4>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>