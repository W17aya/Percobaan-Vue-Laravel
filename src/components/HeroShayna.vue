<template>
    <div>
       <!-- Hero Section Begin -->
    <section class="hero-section">
        <carousel class="hero-items" :items-to-show="1">
            <slide v-for="slide in 10" :key="slide">
                <div class="single-hero-items set-bg" data-setbg="img/hero-1.jpg">
                <div class="container">
                    <div class="row">
                        <div class="col-lg-5">
                            <span>Bag,kids</span>
                            <h1>Black friday</h1>
                            <p>
                                Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore
                            </p>
                            <a href="#" class="primary-btn">Shop Now</a>
                        </div>
                    </div>
                </div>
            </div>
                </slide>
                <template #addons>
        <navigation />
        <pagination />
      </template>

          
        </carousel>
    </section>
    <!-- Hero Section End -->
    </div>
</template>

<script>

import "vue3-carousel/dist/carousel.css";
import {Carousel, Slide, Pagination, Navigation} from "vue3-carousel";


export default {
    name:"Heroshayna",
    components: {
        Carousel,
        Slide,
        Pagination,
        Navigation
    }
};
</script>