<template>
  <div class="container py-24">
    <div class="flex justify-between items-center">
      <div class="flex gap-10 items-center">
        <p class="text-[16px] leading-[19.2px] tracking-[3%] text-[#181A20] font-[600]">(02)</p>
        <h3 class="text-[16px] leading-[19.2px] tracking-[3%] text-[#181A20] font-[600]"> Latest Projexts</h3>
      </div>
      <div class="mr-48 text-start media_title">
        <p class=" font-[500] text-[16px] leading-[19.2px] tracking-[3% ]">
          Featured Communities <br>
          Ciio. Properties
        </p>
      </div>
    </div>

    <div class="container media_container py-12 p-[100px]">
      <swiper
          :slidesPerView="1"
          :spaceBetween="30"
          :keyboard="{
      enabled: true,
    }"
          :autoplay="{
      delay: 2500,
      disableOnInteraction: false,
    }"


          :modules="modules"
          class="mySwiper"
      >
        <swiper-slide>
          <img src="../assets/images/oval-2.png" class="w-[783.25px] h-[500px]" alt="no image">
        </swiper-slide>
        <swiper-slide>
          <img src="../assets/images/oval-2.png" class="w-[783.25px] h-[500px]" alt="no image">
        </swiper-slide>
        <swiper-slide>
          <img src="../assets/images/oval-2.png" class="w-[783.25px] h-[500px]" alt="no image">
        </swiper-slide>
        <swiper-slide>
          <img src="../assets/images/oval-2.png" class="w-[783.25px] h-[500px]" alt="no image">
        </swiper-slide>
        <swiper-slide>
          <img src="../assets/images/oval-2.png" class="w-[783.25px] h-[500px]" alt="no image">
        </swiper-slide>
        <swiper-slide>
          <img src="../assets/images/oval-2.png" class="w-[783.25px] h-[500px]" alt="no image">
        </swiper-slide>
        <swiper-slide>
          <img src="../assets/images/oval-2.png" class="w-[783.25px] h-[500px]" alt="no image">
        </swiper-slide>
        <swiper-slide>
          <img src="../assets/images/oval-2.png" class="w-[783.25px] h-[500px]" alt="no image">
        </swiper-slide>
      </swiper>
    </div>
    <div class="absolute -ml-[20px] top-[1700px] media_text  z-50 flex">
      <p class="font-[400] text-[128px] text-[#181A20]"> the <span class="#686569">Bee</span></p>
    </div>
    <div class="absolute ml-[81%] top-[1700px] media_text z-50 flex">
      <p class="font-[400] text-[128px] text-[#181A20]"> the </p>
    </div>

    <div class="flex justify-between items-center py-4 container text_media">
      <div>
        <p class="font-[400] text-[16px] leading-[19.2px] tracking-[3%] text-[#7D7D7D] mb-4">Affordable Units Starting</p>
        <h2 class="font-[400] text-[50px] leading-[50px] text-[#000000]">
          From $186,000
        </h2>
      </div>

      <div>
        <p class="font-[400] text-[16px] leading-[19.2px] tracking-[3%] text-[#7D7D7D]">
          555 North 400 West <br>
          Centerville, Utah 84014
        </p>
      </div>

      <div>
        <p class="font-[400] text-[16px] leading-[19.2px] tracking-[3%] text-[#7D7D7D]">
          50 Modern Townhomes <br>
          Now Selling
        </p>

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
import {Keyboard,  Pagination, Navigation, Autoplay} from 'swiper/modules';

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Autoplay, Keyboard, Pagination, Navigation],
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
  background: #fff;

  /* Center slide text vertically */
  display: flex;
  justify-content: center;
  align-items: center;
}

.swiper-slide img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
}

@media(max-width: 1200px){
  .media_text{
    display: none;
  }
  .container{
    padding: 4px;
    margin-top: 20px;
  }
}

@media(max-width: 1016px){
  .media_text{
    display: none;
  }
  .container{
    padding: 0;
    margin-top: 20px;
  }
}

@media(max-width: 762px){
  .media_text{
    display: none;
  }
  .container{
    padding: 0;
    margin-top: 20px;
  }
}

@media(max-width: 580px) {
  .media_title {
    margin: 20px;
  }
  .text_media{
    margin: 5px;
    gap: 10px;
  }
  .text_media h2{
  font-size: 30px;
  }
  .text_media p{
    font-size: 20px;
  }
}

@media(max-width: 364px) {

  .text_media{
    display: flex;
    flex-direction: column;
    gap: 15px;
    align-items: start;
    justify-content: start;
  }
}

</style>