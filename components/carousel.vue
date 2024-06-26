<template>

  <div class="container py-24">

    <div class="flex justify-between items-center mb-20">
      <div class=" flex gap-[5rem]">
        <p class="font-[500] text-[16px] leading-[19.2px] tracking-[3%]">(04)</p>
        <span class="font-[500] text-[16px] leading-[19.2px] tracking-[3%]">We build community.</span>
      </div>

      <div>
        <p class="font-[500] text-[16px] leading-[19.2px] tracking-[3%]">Wherever we build, <br>
          we make it better.</p>
      </div>

      <div>
        <div>
          <NuxtLink to="/modern" class="button arrow flex items-center gap-5 cursor-pointer">
            <p class="text-black text-[16px] font-[600]">
              About us
            </p>
          </NuxtLink>
        </div>
      </div>
    </div>

    <div class=" media_flex grid grid-cols-1 sm:grid-cols-2 gap-8 place-items-center">
      <swiper
          :pagination="{
      type: 'fraction',
    }"
          :autoplay="{
      delay: 2500,
      disableOnInteraction: false,
    }"

          :modules="modules"
          class="mySwiper text-[40px] text-white font-parisienne"
      >
        <swiper-slide>
          <img src="../assets/images/glass-man.png"
               class="w-[570px] h-[792px] bg-gradient-to-r from-stone-950 to-gray-700" alt="no image">
        </swiper-slide>
        <swiper-slide><img src="https://images.unsplash.com/photo-1514588645531-00b8822ad997?q=80&w=1935&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" class="w-[570px] h-[792px]" alt="no image"></swiper-slide>
        <swiper-slide>
          <img src="https://images.unsplash.com/photo-1514300971-c747b1ff6d5a?q=80&w=1535&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
               class="w-[570px] h-[792px]" alt="no image">
        </swiper-slide>
        <swiper-slide>
          <img src="https://images.unsplash.com/photo-1548191194-b3d4f051fd7d?q=80&w=1887&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
               class="w-[570px] h-[792px]" alt="no image">
        </swiper-slide>
      </swiper>

      <div class="media_text">
        <p class="text-[50px] font-[400] leading-[50px]">
          Our aim is to build micro-communities that enrich and fortify local areas, turning every space into an opportunity through well-planned land use and design, fostering exploration and growth with a positive impact on existing communities.
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
import { Pagination, Navigation, Autoplay } from 'swiper/modules';

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Autoplay, Pagination, Navigation],
    };
  },
};
</script>

<style lang="scss" scoped>
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

  object-fit: cover;
}


a.button {
  margin: 20px;
  font-size: 20px;
}

.arrow {
  color: #FE7B1E;
  background-color: transparent;
  margin: 4em 0;

  &::after {
    display: inline-block;
    padding-left: 8px;
    content: "\0279E"; // arrow right unicode
    -webkit-transition: transform 0.3s ease-out;
    -moz-transition: transform 0.3s ease-out;
    -ms-transition: transform 0.3s ease-out;
    -o-transition: transform 0.3s ease-out;
    transition: transform 0.3s ease-out;
  }

  &:hover {
    color: #FE7B1E;
    background-color: transparent;

    &::after {
      -webkit-transform: translateX(4px);
      -moz-transform: translateX(4px);
      -ms-transform: translateX(4px);
      -o-transform: translateX(4px);
      transform: translateX(4px);
    }
  }
}

@media(max-width: 1200px){
  .container{
    padding: 10px;
    max-width: 1200px;
  }

  .media_text p{
    font-size: 40px;
  }
}

@media(max-width: 824px){
  .container{
    padding: 5px;
    max-width: 824px;
  }

  .media_text p{
    font-size: 40px;
  }
}

@media(max-width: 720px){
  .container{
    padding: 5px;
    max-width: 720px;
  }

  .media_flex{
    display: flex;
    flex-direction: column;
  }

  .media_text p{
    font-size: 40px;
  }
}
</style>

