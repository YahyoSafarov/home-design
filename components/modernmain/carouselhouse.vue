<template>

  <div class="bg-[#F4F1E7]">
    <div class="container py-24">
      <div class="py-12 mb-20 text_media">
        <h1 class="text-[400] text-[120px] leading-[116px]">theBee More <br> house 6 Photo</h1>
      </div>
      <div class=" slide_media grid grid-cols-1 gap-5 sm:grid-cols-2 md:grid-cols-3">
        <swiper
            :pagination="{
             type: 'fraction',
            }"
            :autoplay="{
             delay: 2500,
             disableOnInteraction: false,
            }"
            :effect="'coverflow'"
            :modules="modules"
            :coverflowEffect="{
             rotate: 10,
             stretch: 0,
             depth: 100,
             modifier: 1 ,
             slideShadows: true,
           }"
            class="mySwiper text-[43.84px] leading-[43.84px] text-white font-parisienne"
        >
          <swiper-slide>
            <img src="../../assets/images/house-1.png" alt="no image">
          </swiper-slide>
          <swiper-slide>
            <img src="https://images.unsplash.com/photo-1615971677499-5467cbab01c0?q=80&w=1780&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
          </swiper-slide>
          <swiper-slide>
            <img src="https://plus.unsplash.com/premium_photo-1661779601614-9206e0451077?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
          </swiper-slide>
          <swiper-slide><img src="https://plus.unsplash.com/premium_photo-1680638265554-bc1e3dec50dd?q=80&w=1932&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image"></swiper-slide>
          <swiper-slide>
            <img src="https://plus.unsplash.com/premium_photo-1679944451403-387670e6e9f7?q=80&w=2047&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
          </swiper-slide>
          <swiper-slide>
            <img src="https://plus.unsplash.com/premium_photo-1678719544833-a4eda1a344a0?q=80&w=2003&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
          </swiper-slide>
        </swiper>

        <swiper
            :pagination="{
             type: 'fraction',
            }"
            :autoplay="{
             delay: 2500,
             disableOnInteraction: false,
            }"
            :effect="'coverflow'"
            :modules="modules"
            :coverflowEffect="{
             rotate: 10,
             stretch: 0,
             depth: 100,
             modifier: 1 ,
             slideShadows: true,
           }"
            class="mySwiper text-[43.84px] leading-[43.84px] text-white font-parisienne"
        >
          <swiper-slide>
            <img src="../../assets/images/house-2.png" alt="">
          </swiper-slide>
          <swiper-slide>
            <img src="https://plus.unsplash.com/premium_photo-1661876449499-26de7959878f?q=80&w=1974&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
          </swiper-slide>
          <swiper-slide>
            <img src="https://plus.unsplash.com/premium_photo-1687960116647-70ef7323dde8?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
          </swiper-slide>
          <swiper-slide>
            <img src="https://plus.unsplash.com/premium_photo-1661883982941-50af7720a6ff?q=80&w=1974&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
          </swiper-slide>
          <swiper-slide>
            <img src="https://plus.unsplash.com/premium_photo-1680300960892-bd11b59b469b?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
          </swiper-slide>
          <swiper-slide>
            <img src="https://plus.unsplash.com/premium_photo-1686782502706-7d78d6b42b63?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
          </swiper-slide>
        </swiper>

        <swiper
            :pagination="{
             type: 'fraction',
             clickable: true,
            }"
            :autoplay="{
             delay: 2500,
             disableOnInteraction: false,
            }"
            :effect="'coverflow'"
            :modules="modules"
            :coverflowEffect="{
             rotate: 10,
             stretch: 0,
             depth: 100,
             modifier: 1 ,
             slideShadows: true,
           }"
            class="mySwiper text-[43.84px] leading-[43.84px] text-white font-parisienne"
        >
          <swiper-slide>
            <img src="../../assets/images/house-3.png" alt="no image">
          </swiper-slide>
          <swiper-slide>
            <img src="https://plus.unsplash.com/premium_photo-1663059604652-4510a42c8490?q=80&w=2072&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
          </swiper-slide>
          <swiper-slide>
            <img src="https://plus.unsplash.com/premium_photo-1683880731495-ae0f4bf18c7e?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
          </swiper-slide>
          <swiper-slide>
            <img src="https://plus.unsplash.com/premium_photo-1683140959696-99dfefadc6bb?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
          </swiper-slide>
          <swiper-slide><img src="https://plus.unsplash.com/premium_photo-1675195901141-1fe9d762d1f0?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image"></swiper-slide>
          <swiper-slide>
            <img src="https://plus.unsplash.com/premium_photo-1697651368986-58f5368a946a?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
          </swiper-slide>
        </swiper>
      </div>
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
import { Autoplay,  EffectCoverflow, Pagination, Navigation } from 'swiper/modules';

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Autoplay, EffectCoverflow, Pagination, Navigation],
    };
  },
};
</script>

<style scoped>
.swiper {
  width: 100%;
  height: 100%;
}
.mySwiper{
  display: flex;
  flex-direction: column;
}

.swiper-slide {
  text-align: center;
  font-size: 18px;
  background: #fff;

  /* Center slide text vertically */
  display: flex;
  justify-content: center;
  align-items: center;
}

.swiper-slide img {
  display: block;
  width: 614.11px;
  height: 613.46px;
  object-fit: cover;
}

@media(max-width: 1200px){
  .container{
    padding: 10px;
    max-width: 1200px;
  }
  .text_media h1{
    font-size: 90px !important;
  }
}

@media(max-width: 950px){
  .container{
    padding: 10px;
    max-width: 950px;
  }
  .text_media h1{
    font-size: 90px !important;
  }
  .slide_media{
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px));
  }
}
</style>
