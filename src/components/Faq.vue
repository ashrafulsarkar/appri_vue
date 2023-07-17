<script setup>
const faqs = [
    {
        title: 'How to Buy This?',
        desc: 'Enables you to define cross-channel profiles and improve audience. sessions per week There is no one type or way in our diverse'
    },
    {
        title: 'It is refundable?',
        desc: 'Enables you to define cross-channel profiles and improve audience. sessions per week There is no one type or way in our diverse'
    },
    {
        title: 'Can i use free',
        desc: 'Enables you to define cross-channel profiles and improve audience. sessions per week There is no one type or way in our diverse'
    },
]

const uniqueId = index =>  `heading_${index}`
const uniquetext = index => `collapse_${index}`
const uniquetextID = uniquetext =>  `#${uniquetext}`
</script>
<template>
    <!-- faq-bg-items-area start -->
    <section class="faq-bg-items">
        <!--faq-area-->
        <div id="faq" class="faq-area">
            <div class="container">
                <div class="row">
                    <div class="col-xl-12">
                        <div class="section-title text-center pb-80">
                            <h2>FAQS</h2>
                            <p>Enables you to define cross-channel profiles and improve audience. sessions per week</p>
                        </div>
                    </div>
                </div>
                <div class="row">
                    <div class="col-xl-5 col-lg-5 col-md-5">
                        <div class="faq-img">
                            <img src="/img/app/faq-app.png" alt="">
                        </div>
                    </div>
                    <div class="col-xl-7 col-lg-7 col-md-7">
                        <div class="how-buy">
                            <div class="accordion" id="accordionExample">
                                <div class="card" v-for="(faq,index) in faqs">
                                    <div class="card-header" :id="uniqueId(index)">
                                        <h2 class="mb-0">
                                            <button class="btn btn-link" :class="0==index?'':'collapsed'" type="button" data-toggle="collapse" :data-target="uniquetextID(uniquetext(index))" :aria-expanded="0==index?'true':'false'" :aria-controls="uniquetext(index)">
                                                {{ faq.title }}
                                            </button>
                                        </h2>
                                    </div>
                                    <div :id="uniquetext(index)" class="collapse" :class="0==index?'show':''" :aria-labelledby="uniqueId(index)" data-parent="#accordionExample">
                                        <div class="card-body">
                                            {{ faq.desc }}
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>