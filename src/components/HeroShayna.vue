<template>
    <!-- Hero Section Begin -->
 <section class="hero-section">
     <carousel :autoplay="2000" wrap-around="true" :items-to-show="1">
             <Slide v-for="slide in 10" :key="slide">
             <div class="single-hero-items set-bg" style="background-image: url('img/hero-1.jpg')">
             <div class="container">
                 <div class="row banner-info">
                        <div class="col-lg-5"> 
                            <span class="primary-btn" >bag, kids </span>
                            <h1>Black friday</h1>
                            <p>
                                Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore
                            </p>
                            <a href="#" class="primary-btn">Shop Now</a>
                        </div>
                    </div>
                </div>
            </div>
            <!-- <div class="single-hero-items set-bg" style="background-image: url('/img/hero-2.jpg')">
          <div class="container">
            <div class="row">
                <div class="row banner-info">
              <div class="col-lg-5">
                <span>Bag,kids</span>
                <h1>Black friday</h1>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore</p>
                <a href="#" class="primary-btn">Shop Now</a>
              </div>
            </div>
          </div>
        </div> -->
             </slide>
                <template #addons>
        <navigation />
        <pagination />
      </template>
        </carousel>
    </section>
    <!-- Hero Section End -->
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

<style>
.set-bg{
    width: 100%;
    height: 500px;
}

.banner-info{
    margin-top: 130px;
}
.banner-text{
    color: fffff;
    size: 13px;
}
</style>