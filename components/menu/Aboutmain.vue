<template>
  <div class="container py-24">
    <div class="flex gap-10 mb-10">
      <p class="font-[500] text-[16px] leading-[19.2px] tracking-[3%]">(02)</p>
      <h1 class="font-[400] text-[50px] leading-[50px]">Process Makes <br>
        perfect</h1>
    </div>

    <div class="grid grid-cols-1 container md:grid-cols-2 xl:grid-cols-4 gap-8">
      <div v-for="p in products" :key="p">
        <div class="card space-y-3 sm:space-y-4 cursor-pointer">
          <NuxtLink :to="`/products/${p.id}`" class="container">
            <div class="flex gap-4 items-center">
              <h1 class="text-[32px] font-[400] leading-[40px] text-black">{{ p.name }}</h1>
              <p class="text-black">
                {{ p.title }}
              </p>
            </div>

            <p class="text-black">
              {{p.description}}
            </p>

          </NuxtLink>

          <!-- <ProductCard :product = "p"/> -->
        </div>
      </div>
    </div>

    <div>
      <div class="gallery-container">
        <img src="https://images.unsplash.com/photo-1513584684374-8bab748fbf90?q=80&w=2065&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
        <img src="https://images.unsplash.com/photo-1604014238170-4def1e4e6fcf?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
        <img src="https://images.unsplash.com/photo-1600047509358-9dc75507daeb?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
        <img src="https://images.unsplash.com/photo-1600563438938-a9a27216b4f5?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">

      </div>
    </div>
  </div>
</template>

<script setup>
const products = [
  {
    id: 1,
    name: "01",
    title:
        "/ Gather Talent",
    price: 109.95,
    description:
        "At the outset, we search for the crème de la crème. Our communities are conceptualized and developed by a combination of established and rising talent who are driven, modest, and astute. They recognize that this is not just a temporary project, but a progression.",
  },
  {
    id: 2,
    name: "02",
    title:
        "/ Gather Talent",
    price: 109.95,
    description:
        "We discern potential in the underutilized areas of thriving neighborhoods. Then, through judicious land planning, we devise a blueprint that will generate beneficial outcomes, intelligent expansion, and advancement in these regions.",
  },
  {
    id: 3,
    name: "03",
    title:
        "/ Gather Talent",
    price: 109.95,
    description:
        "Our talented in-house design team constitutes one of our major strengths. With meticulous attention to detail and strategic utilization of texture, flow, form, and finishes, they assist us in constructing breathtaking pieces of architecture that become the dwelling our clients call home.",
  },
  {
    id: 4,
    name: "04",
    title:
        "/ Gather Talent",
    price: 109.95,
    description:
        "Our in-house builders carry out every community design with an emphasis on quality and sustainability.",
  },
];
</script>

<style lang="scss" scoped>
@keyframes gallery {
  0%{
    opacity: 1;
  }
  25%{
    opacity: 0;
  }
  50%{
    opacity: 0;
  }
  75%{
    opacity: 0;
  }
  100%{
    opacity: 1;
  }
}

.gallery-container{
  position: relative;
  max-width: 1000px;
  height: 450px;
  overflow: hidden;
  margin: 50px auto 0 auto;
  tranform: translate3d(0,0,0);
}

img {
  position: absolute;
  top: 0;
  left: 50%;
  margin-left: -50%;
  max-width: 100%;
  width: 1000px;
  height: 700px;
  object-fit: cover;
  animation-name: gallery;
  animation-duration: 10s;
  animation-iteration-count: infinite;
  animation-direction: alternate;
  animation-timimg-function: linear;
}

img:nth-of-type(1){
  z-index: 4;
}

img:nth-of-type(2){
  animation-delay: 2.5s;
  z-index: 3;
}

img:nth-of-type(3){
  animation-delay: 5s;
  z-index: 2;
}

img:nth-of-type(4){
  animation-delay: 7.5s;
  z-index: 1;
}



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

</style>