<script setup>
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
//import { Carousel, Slide } from 'vue-carousel';
import 'vue3-carousel/dist/carousel.css';
import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel';

</script>

<template>
    <Header class="fixed top-0 left-0 w-full z-20" />
    <main>
        <section class="h-screen w-full">
            <carousel class="h-screen w-full" :items-to-show="1" :wrap-around="true" :autoplay="5000" :transition="500">
                <slide :key="1" class="h-screen">
                    <img src="./assets/placeholders/black-4906807.jpg" alt="placeholder 1" class="h-full w-full object-cover object-bottom">
                </slide>
                
                <slide :key="2" class="h-screen">
                    <img src="./assets/placeholders/breakdancing-511922.jpg" alt="placeholder 1" class="h-full w-full object-cover object-bottom">
                </slide>

                <slide :key="3" class="h-screen">
                    <img src="./assets/placeholders/girls-6908871.jpg" alt="placeholder 1" class="h-full w-full object-cover object-bottom">
                </slide>

                <slide :key="4" class="h-screen">
                    <img src="./assets/placeholders/high-school-1579517.jpg" alt="placeholder 1" class="h-full w-full object-cover object-bottom">
                </slide>
            </carousel>
            <!--
            <carousel :per-page="1" :navigate-to="someLocalProperty" :mouse-drag="false">
                <slide>
                    Slide 1 Content
                </slide>
                <slide>
                    Slide 2 Content
                </slide>
            </carousel>-->
            <!--
            <Carousel :per-page="1">
                <Slide>
                    <img src="./assets/placeholders/black-4906807.jpg" alt="placeholder 1" class="snap-center h-full w-full object-cover object-bottom flex-shrink-0">
                </Slide>
                <Slide>
                    <img src="./assets/placeholders/breakdancing-511922.jpg" alt="placeholder 1" class="snap-center h-full w-full object-cover object-center flex-shrink-0">
                </Slide>
                <Slide>
                    <img src="./assets/placeholders/girls-6908871.jpg" alt="placeholder 1" class="snap-center h-full w-full object-cover object-bottom flex-shrink-0">
                </Slide>
                <Slide>
                    <img src="./assets/placeholders/high-school-1579517.jpg" alt="placeholder 1" class="snap-center h-full w-full object-cover object-bottom flex-shrink-0">
                </Slide>
            </Carousel>
        -->
        </section>
    </main>
    <Footer />
</template>