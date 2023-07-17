<script setup>
const features = [
    {title: 'Easy Customize', details: 'Enables you to define cross-channel profiles and improve audience. sessions per week', img: '/img/features/features1.png'},
    {title: 'Easy Customize', details: 'Enables you to define cross-channel profiles and improve audience. sessions per week', img: '/img/features/features2.png'},
    {title: 'Easy Customize', details: 'Enables you to define cross-channel profiles and improve audience. sessions per week', img: '/img/features/features3.png'}
]
</script>
<template>
    <!-- features area start -->
    <section id="features" class="features-area pt-120 pb-270">
        <div class="features-shape d-none d-md-block">
            <img src="/img/shape/feature-shape1.png" alt="" class="feature-shape1">
            <img src="/img/shape/feature-shape2.png" alt="" class="feature-shape2">
        </div>
        <div class="container">
            <div class="row">
                <div class="col-xl-12">
                    <div class="section-title text-center pb-70">
                        <h2>Unique Features</h2>
                        <p>Enables you to define cross-channel profiles and improve audience. sessions per week</p>
                    </div>
                </div>
            </div>
            <div class="row">
                <div class="col-xl-4 col-lg-4 col-md-4" v-for="(feature, index) in features" :key="index">
                    <div class="single-features text-center mb-30">
                        <div class="features-img pb-45">
                            <img :src="feature.img" :alt="feature.title">
                        </div>
                        <div class="features-text">
                            <h4>{{ feature.title }}</h4>
                            <p>{{ feature.details }}</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>