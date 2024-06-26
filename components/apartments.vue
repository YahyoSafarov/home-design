<template>
  <div class="bg-[#DFD8BF]">
    <div class="container py-10 pb-14">
      <div class="flex gap-[5rem] mb-14">
        <p class="text-[16px] font-[500] leading-[19.2px] tracking-[3%]">(03)</p>
        <h3 class="text-[16px] font-[500] leading-[19.2px] tracking-[3%]">i.m looking for:</h3>
      </div>

      <div class="flex justify-between items-center mb-14">
        <div class="media_text">
          <h1 class="text-[128px] font-[400] leading-[154px]">Apartments</h1>
        </div>

        <div>
          <div class="scroll-down mr-10">
            <span></span>
            <span></span>
            <span></span>
          </div>
        </div>
      </div>

      <div class=" media_wrap grid grid-cols-1 gap-3 sm:grid-cols-2 md:grid-cols-3">
        <div
            id="card"
            class="p-4  transition-all duration-500 hover:shadow-xl dark:bg-slate-950"
        >
          <div class="overflow-hidden">
            <img
                src="../assets/images/apartments-1.png"
                alt="No image"
                class="mx-auto h-[280px] w-full transition duration-700 hover:skew-x-2 hover:scale-110"
            />
          </div>
          <div class="flex items-center gap-28">
            <div class="flex flex-col pt-2 text-slate-600">
              <p class="text-[16px] font-[400] text-[#262626]">theBEVERLY</p>
              <p class="line-clamp-1 text-[12px]"> Salt Lake City</p>
            </div>

            <div class="space-y-3 py-3">
              <h1 class="line-clamp-1 text-[16px] font-[400]">
                Now Leasing
              </h1>
              <p class="line-clamp-2">
                Apartments / Starting From — <br> $1,675+ Monthly
              </p>
            </div>
          </div>
        </div>
        <div
            id="card"
            class="p-4  transition-all duration-200 hover:shadow-xl dark:bg-slate-950"
        >
          <div class="overflow-hidden">
            <img
                src="../assets/images/apartments-2.png"
                alt="No image"
                class="mx-auto h-[280px] w-full  transition duration-700 hover:skew-x-2 hover:scale-110"
            />
          </div>
          <div class="flex items-center gap-28">
            <div class="flex flex-col pt-2 text-slate-600">
              <p class="text-[16px] font-[400] text-[#262626]">theBEVERLY</p>
              <p class="line-clamp-1 text-[12px]"> Salt Lake City</p>
            </div>

            <div class="space-y-3 py-3">
              <h1 class="line-clamp-1 text-[16px] font-[400]">
                Now Leasing
              </h1>
              <p class="line-clamp-2">
                Apartments / Starting From — <br> $1,675+ Monthly
              </p>
            </div>
          </div>

        </div>
        <div
            id="card"
            class="p-4  transition-all duration-200 hover:shadow-xl dark:bg-slate-950"
        >
          <div class="overflow-hidden">
            <img
                src="../assets/images/apartments-3.png"
                alt="No image"
                class="mx-auto h-[280px] w-full transition duration-700 hover:skew-x-2 hover:scale-110"
            />
          </div>
          <div class="flex items-center gap-28">
            <div class="flex flex-col pt-2 text-slate-600">
              <p class="text-[16px] font-[400] text-[#262626]">theBEVERLY</p>
              <p class="line-clamp-1 text-[12px]"> Salt Lake City</p>
            </div>

            <div class="space-y-3 py-3">
              <h1 class="line-clamp-1 text-[16px] font-[400]">
                Now Leasing
              </h1>
              <p class="line-clamp-2">
                Apartments / Starting From — <br> $1,675+ Monthly
              </p>
            </div>
          </div>

        </div>
      </div>
    </div>
  </div>
</template>

<script setup>

</script>

<style scoped>

.scroll-down
{

}
.scroll-down span:nth-child(2)
{
  animation-delay: -0.2s;
}
.scroll-down span:nth-child(3)
{
  animation-delay: -0.4s;
}
.scroll-down span
{
  display: block;
  width: 20px;
  height: 20px;
  border-bottom: 4px solid #000;
  border-right: 4px solid #000;
  transform: rotate(45deg);
  margin: -10px;
  animation: animate 2s infinite;
}
@keyframes animate
{
  0%
  {
    opacity: 0;
    transform: rotate(45deg) translate(-20px,-20px);
  }
  50%
  {
    opacity: 1;
  }
  100%
  {
    opacity: 0;
    transform: rotate(45deg) translate(20px,20px);
  }
}

@media(max-width: 1200px){
  .container{
    padding: 10px;
    max-width: 1200px;
  }
  .media_text h1{
    font-size: 90px;
  }

  .media_wrap{
  }
}

@media(max-width: 929px){
  .container{
    padding: 10px;
    max-width: 929px;
  }
}

@media(max-width: 845px){
  .container{
    padding: 5px;
    max-width: 929px;
  }
  .media_wrap{
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px));
  }
}

@media(max-width: 530px){
  .media_text h1{
    font-size: 50px;
  }
}
</style>