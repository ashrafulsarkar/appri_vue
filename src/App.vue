<script setup>
import Footer from './components/Footer.vue'
import AvailableApp from './components/AvailableApp.vue'
import Subscribe from './components/Subscribe.vue'
import News from './components/News.vue'
import Faq from './components/Faq.vue'
import Screenshort from './components/Screenshort.vue'
import Price from './components/Price.vue'
import Video from './components/Video.vue'
import Features from './components/Features.vue'
import Counter from './components/Counter.vue'
import Hero from './components/Hero.vue'
import Header from './components/Header.vue'

</script>

<template>
  <Header></Header>
  <main>
    <Hero></Hero>
    <Counter></Counter>
    <Features></Features>
    <Video></Video>
    <Price></Price>
    <Screenshort></Screenshort>
    <Faq></Faq>
    <News></News>
    <Subscribe></Subscribe>
    <AvailableApp></AvailableApp>
  </main>
  <Footer></Footer>
</template>

<style scoped></style>
