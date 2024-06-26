<template>
  <div class="">
    <div
        class="py-12 sm:py-0 dark:bg-black dark:text-white duration-300 overflow-hidden m"
    >
      <div class="container p-8 min-h-[700px] flex relative">
        <div
            class="grid grid-cols-1 sm:grid-cols-2 gap-6 place-items-center relative"
        >


          <div class="order-2 con sm:order-1 title space-y-5">
            <h1 class="text-[103px] font-normal text-[#181A20]">
              ___theBee <br>
              are 80 <span class="font-[700]">Modern</span>  Townhomes
            </h1>

            <div class="flex gap-6 ml-4">
              <div class="flex gap-5">
                <img src="../../assets/images/map-location.svg" class="w-[28px] h-[35.5px]" alt="no map">
                <p class="font-[400] text-[32px] leading-[40px]">Los Angels, USA</p>
              </div>
<!--              <div class='pin'></div>-->
<!--              <div class='pulse'></div>-->
            </div>
          </div>

          <div data-aos="fade-up" data-aos-offset="0" class="order-1 sm:order-2">
            <img src="../../assets/images/modern-home.png"  alt="no image" class="" />
          </div>
        </div>



      </div>
    </div>
  </div>

</template>

<script setup></script>

<style lang="scss" scoped>


.home_shape-big-1 {
  background-color: #ff662d;
  top: 40rem;
  left: -9.5rem;
}

.home_shape-bg {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  mix-blend-mode: soft-light;
  opacity: 0.3;
}

button {
  display: inline-block;
  border-radius: 16px;
  padding: 16px 32px 16px 32px;
  color: #fff;
  background: #ff662d;
  font-size: 20px;
  transition: 0.5s ease;
}
button:hover {
  background: transparent;
  color: #ff662d;
  box-shadow: 0 0 20px #ff662d;
}


.pin{
  width: 30px;
  height: 30px;
  border-radius: 50% 50% 50% 0;
  background: #89849b;
  position: absolute;
  transform: rotate(-45deg);
  left: 50%;
  top: 50%;
  margin: -20px 0 0 -20px;
  animation-name: bounce;
  animation-fill-mode: both;
  animation-duration: 1s;

  &:after{
    content: '';
    width: 14px;
    height: 14px;
    margin: 8px 0 0 8px;
    background: #2F2F2F;
    position: absolute;
    border-radius: 50%;
  }

  .pulse{
    background: rgba(0,0,0,0.9);
    border-radius: 50%;
    height: 14px;
    width: 14px;
    position: absolute;
    left: 50%;
    top: 50%;
    margin: 11px 0 0 -12px;
    transform: rotateX(55deg);
    z-index: -2;

    &:after{
      content: "";
      border-radius: 50%;
      height: 40px;
      width: 40px;
      position: absolute;
      margin: -13px 0 0 -13px;
      animation: pulsate 1s ease-out;
      animation-iteration-count: infinite;
      opacity: 0.0;
      box-shadow: 0 0 1px 2px #89849b;
      animation-delay: 1.1s;
    }
  }

  @keyframes pulsate{
    0%{
      transform: scale(0.1, 0.1);
      opacity: 0.0;
    }
    50%{
      opacity: 1.0;
    }
    100%{
      transform: scale(1.2, 1.2);
      opacity: 0;
    }
  }

  @keyframes bounce{
    0%{
      opacity: 0;
      transform: translateY(-2000px) rotate(-45deg);
    }
    80%{
      transform: translateY(-10px) rotate(-45deg);
    }
    100%{
      transform: translateY(0) rotate(-45deg);
    }
  }

}

@media(max-width: 1200px){
  /* .m{
    display: flex;
    align-items: center;
    justify-content: center;
  } */

}
@media(max-width: 500px){
  .title h1{
    font-size: 45px;
  }

}

</style>
