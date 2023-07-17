<script setup>
const Prices = {
    monthly: [
        {
            title: 'Primary',
            price: 0,
            package: ['1GB storage', '1 project limit', '2 contributors limit', 'Unlimited viewers', 'Team account'],
            url: '#'
        },
        {
            title: 'Popular',
            price: 10,
            package: ['1GB storage', '1 project limit', '2 contributors limit', 'Unlimited viewers', 'Team account'],
            url: '#'
        },
        {
            title: 'Premium',
            price: 15,
            package: ['1GB storage', '1 project limit', '2 contributors limit', 'Unlimited viewers', 'Team account'],
            url: '#'
        }
    ],
    yearly: [
        {
            title: 'Primary',
            price: 25,
            package: ['1GB storage', '1 project limit', '2 contributors limit', 'Unlimited viewers', 'Team account'],
            url: '#'
        },
        {
            title: 'Popular',
            price: 100,
            package: ['1GB storage', '1 project limit', '2 contributors limit', 'Unlimited viewers', 'Team account'],
            url: '#'
        },
        {
            title: 'Premium',
            price: 150,
            package: ['1GB storage', '1 project limit', '2 contributors limit', 'Unlimited viewers', 'Team account'],
            url: '#'
        }
    ],
}
</script>
<template>
    <!-- price area start -->
    <section id="pricing" class="price-area pt-60">
        <div class="container">
            <div class="row">
                <div class="col-xl-12 pb-80">
                    <div class="section-title text-center">
                        <h2>Pricing Plan</h2>
                        <p>Enables you to define cross-channel profiles and improve audience. sessions per week</p>
                    </div>
                </div>
            </div>
            <div class="price-tab">
                <div class="price-menu-box text-center">
                    <ul class="nav price-tabs" id="myTab" role="tablist">
                        <li class="nav-item">
                            <a class="nav-link active" id="monthly-tab" data-toggle="tab" href="#monthly" role="tab" aria-controls="monthly" aria-selected="true">Monthly</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" id="yearly-tab" data-toggle="tab" href="#yearly" role="tab" aria-controls="yearly" aria-selected="false">Yearly</a>
                        </li>
                    </ul>
                    <div class="tab-content" id="myTabContent">
                        <div class="tab-pane fade show" :class="0==index?'active':''" v-for="(Price, property, index) in Prices" :id="property" role="tabpanel" :aria-labelledby="'monthly'==property?'monthly-tab':'yearly-tab'">
                            <div class="row">
                                <div class="col-xl-4 col-lg-4 col-md-4 pb-30" v-for="(item, index) in Price">
                                    <div class="price-box">
                                        <div class="price-header">
                                            <h4>{{ item.title }}</h4>
                                            <h2>${{ item.price }}<span class="sap">/</span><span>{{ 'monthly'==property?'mo':'yr' }}</span>
                                            </h2>
                                        </div>
                                        <div class="price-items">
                                            <ul>
                                                <li v-for="itemlist in item.package">{{ itemlist }}</li>
                                            </ul>
                                        </div>
                                        <div class="price-btn">
                                            <a :href="item.url" class="btn btn-theme-border" :class="1==index?'active':''">Get Started Now</a>
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