<script setup>
const counters = [
    {number:40790, title: 'Download App'},
    {number:1090, title: 'Active Users'},
    {number:790, title: 'Positive Reviews'}
]
</script>
<template>
    <!-- counter area start -->
    <section class="counter-area">
        <div class="container">
            <div class="row counter-full text-center">
                <div class="col-xl-8 col-lg-8 col-md-12 offset-xl-2 offset-lg-2">
                    <div class="row">
                        <div class="col-xl-4 col-lg-4 col-md-4 col-sm-4 pb-30" v-for="(counter,index) in counters" :key="index">
                            <div class="single-counter">
                                <h3 class="counter">{{counter.number}}</h3>
                                <span>{{counter.title}}</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>