<template>
  <div class="bg-[#F4F1E7] py-24 flex items-center justify-center">
    <div class="container">
      <div class="media_title w-3/4 flex gap-20 transform  translate-x-[10%]">
        <h3 class="font-[500] text-[16px]">(01)</h3>
        <p class=" font-[400] text-[50px] leading-[50px] text-[#181A20] whitespace-normal">
          At Achille Ciio, we're paving the path for exceptional real estate in Utah. As a design, build, and development company, our aim is to craft communities that enrich, fortify, and add to the overall fabric of neighboring areas.
        </p>
      </div>
    </div>
  </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>
@media(max-width: 1200px){
  .media_title{
    font-size: 40px;
  }
}

@media(max-width: 1200px){
  .media_title{
    display: flex;
    width: 100%;
  }
  .media_title p{
    display: flex;
    align-items: center;
    justify-content: center;
    text-wrap: balance;
    font-size: 40px;
  }
}

@media(max-width: 764px){
  .media_title{
    display: flex;
    width: 100%;
  }
  .media_title p{
    display: flex;
    align-items: center;
    justify-content: center;
    text-wrap: balance;
    font-size: 35px;
  }
}

@media(max-width: 700px){
  .media_title{
    display: flex;
    width: 100%;
  }
  .media_title p{
    display: flex;
    align-items: center;
    justify-content: center;
    text-wrap: balance;
    font-size: 35px;
    transform: translateX(-15%);
  }
}
</style>