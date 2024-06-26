<template>
  <div class="bg-[#262A34]">
    <div class="container py-12">
      <div class="grid grid-cols-1 sm:grid-cols-2 place-items-center">
        <div class="">
          <img src="https://images.unsplash.com/photo-1492889971304-ac16ab4a4a5a?q=80&w=2074&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
               class="w-[570px] h-[788px] object-cover" alt="no image">

<!--          <div>-->
<!--            <div class="flex items-center justify-center flex-col rounded-[80px] bg-white">-->
<!--              <h3>Open House</h3>-->
<!--              <h3>-->
<!--                September 16-->
<!--              </h3>-->
<!--              <h3>-->
<!--                8.AM — 2.PM-->
<!--              </h3>-->
<!--            </div>-->
<!--            <img src="../../assets/images/Star1.svg" alt="no star">-->
<!--          </div>-->
        </div>


        <div>
          <div class="flex gap-32 py-4 font-[400] text-[16px] leading-[19.2px] tracking-[3%] text-white">
            <p> theBee</p>
            <p>595 N W North Salt Lake, <br>
              UT 84054 THB BUILDING <br>For Lease</p>
          </div>

          <div class="border-b-[1px] w-[470px] border-[#999999]"></div>

          <div class="font-[400] text-[96px] leading-[105.6px] text-white mt-10">
            <h1>Plot 1602</h1>
          </div>

          <div>
            <ul class="flex gap-14 items-center font=[400] text-[16px] leading-[19.2px] tracking-[3%] text-white py-8">
              <li>Now Selling</li>
              <li>Quick Move-In</li>
              <li>December Move-In</li>
            </ul>

            <h1 class="font-[400] text-[96px] leading-[106px] text-white mb-7">
              $650,000
            </h1>
          </div>

          <div>
            <ul class="flex gap-14 items-center text-white font-[400] text-[18px] leading-[21.6px] tracking-[3%]">
              <li>
                beds
                <p>2</p>
              </li>
              <li>
                bath
                <p>2</p>
              </li>
              <li>
               garage
                <p>2</p>
              </li>
              <li>
                fineshed sq ft
                <p>2</p>
              </li>
            </ul>

            <div class="border-b-[1px] w-[470px] border-[#999999] py-4 mb-8"></div>
            <ul class="flex gap-14 items-center text-white font-[400] text-[18px] leading-[21.6px] tracking-[3%]">
              <li>
                beds
                <p>2</p>
              </li>
              <li>
                bath
                <p>2.5</p>
              </li>
              <li>
                garage
                <p>2</p>
              </li>
              <li>
                fineshed sq ft
                <p>1707</p>
              </li>
            </ul>
          </div>

          <div>
            <NuxtLink to="" class="button arrow flex items-center gap-5 py-4 cursor-pointer">
              <p class=" text-[16px] font-[600] text-white">
                Get to know us
              </p>
            </NuxtLink>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>
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
</style>