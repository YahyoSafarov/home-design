<template>
  <div class="bg-[#F0F0F0]">
    <div class="container py-24">
      <swiper
          :pagination="{
      type: 'fraction',
    }"
          :autoplay="{
      delay: 2500,
      disableOnInteraction: false,
    }"
          :modules="modules"
          class="mySwiper text-white font-parisienne text-[40px] leading-[40px]"
      >
        <swiper-slide>
          <img src="https://images.unsplash.com/photo-1507089947368-19c1da9775ae?q=80&w=1776&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
               class="w-[972px] h-[738px]" alt="no image">
        </swiper-slide>
        <swiper-slide>
          <img src="https://images.unsplash.com/photo-1713514022505-fb1f65d476a7?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
               class="w-[972px] h-[738px]" alt="no image">
        </swiper-slide>
        <swiper-slide>
          <img src="https://images.unsplash.com/photo-1517330218601-cd55b21a35af?q=80&w=2071&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
               class="w-[972px] h-[738px]" alt="no image">
        </swiper-slide>
        <swiper-slide>
          <img src="https://plus.unsplash.com/premium_photo-1667520035292-2e1b8fc4280e?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
               class="w-[972px] h-[738px]" alt="no image">
        </swiper-slide>
        <swiper-slide>
          <img src="https://images.unsplash.com/photo-1668910238897-4aec667ff550?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
               class="w-[972px] h-[738px]" alt="no image">
        </swiper-slide>
        <swiper-slide>
          <img src="https://plus.unsplash.com/premium_photo-1706541570171-65707d5a03be?q=80&w=2071&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
               class="w-[972px] h-[738px]" alt="no image">
        </swiper-slide>
      </swiper>
    </div>
  </div>

</template>
<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';

import 'swiper/css/pagination';
import 'swiper/css/navigation';


// import required modules
import {Autoplay, Pagination, Navigation } from 'swiper/modules';

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [ Autoplay, Pagination, Navigation],
    };
  },
};
</script>

<style scoped>
.swiper {
  width: 100%;
  height: 100%;
}

.swiper-slide {
  text-align: center;
  font-size: 18px;

  /* Center slide text vertically */
  display: flex;
  justify-content: center;
  align-items: center;
}

.swiper-slide img {
  display: block;
  object-fit: cover;
}

</style>