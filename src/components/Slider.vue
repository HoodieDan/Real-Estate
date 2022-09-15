<template>
    <swiper
        class="desktop"
        :slides-per-view="3.2"
        :space-between="10"
        navigation
    >
        <swiper-slide><img src="../assets/images/image-1.png" alt="" class="img-fluid"></swiper-slide>
        <swiper-slide><img src="../assets/images/image-2.png" alt="" class="img-fluid"></swiper-slide>
        <swiper-slide><img src="../assets/images/image-3.png" alt="" class="img-fluid"></swiper-slide>
        <swiper-slide><img src="../assets/images/image-1.png" alt="" class="img-fluid"></swiper-slide>
        <swiper-slide><img src="../assets/images/image-2.png" alt="" class="img-fluid"></swiper-slide>
        <swiper-slide><img src="../assets/images/image-3.png" alt="" class="img-fluid"></swiper-slide>
    </swiper>

    <swiper
        class="mobile"
        :modules="[EffectCards]"
        effect="cards"
    >
        <swiper-slide><img src="../assets/images/image-1.png" alt="" class="img-fluid"></swiper-slide>
        <swiper-slide><img src="../assets/images/image-2.png" alt="" class="img-fluid"></swiper-slide>
        <swiper-slide><img src="../assets/images/image-3.png" alt="" class="img-fluid"></swiper-slide>
        <swiper-slide><img src="../assets/images/image-1.png" alt="" class="img-fluid"></swiper-slide>
        <swiper-slide><img src="../assets/images/image-2.png" alt="" class="img-fluid"></swiper-slide>
        <swiper-slide><img src="../assets/images/image-3.png" alt="" class="img-fluid"></swiper-slide>
    </swiper>
  </template>

<script>
// import Swiper core and required modules
import SwiperCore, { Navigation, EffectCards } from 'swiper';

// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';
import 'swiper/css/effect-fade';

SwiperCore.use([ Navigation, EffectCards ])
// Import Swiper styles
export default {
    name: 'Slider',
    data() {
        return {
            number: 2.2
        }
    },
    // mounted () {
    //     if (window.innerWidth > 1115) {
    //         this.number = 3.2
    //     }
    //     if (window.innerWidth >= 1366) {
    //         this.number = 3.2
    //     }
    // },
    components: {
        Swiper,
        SwiperSlide,
    },
    setup() {
      return {
        EffectCards,
      };
    },
};
</script>

<style scoped>
@media (min-width: 576px) {
    .mobile {
        display: none;
    }
}
@media (max-width: 575px) {
    .desktop {
        display: none;
    }
}
</style>
