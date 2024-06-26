<template>
  <div class="bg-[#E0BB68]">
    <div class="container -mt-[2.2%]">
      <div class="grid grid-cols-2 grid_container">
        <div class="flex gap-[4rem] items-center">
          <div>
            <p class="font-[400] text-[22.76px] leading-[28.44px] text-[#181A20]"> 4 Available </p>
          </div>
          <div class=" flex items-center justify-center text-center flex-col w-[120.89px] h-[120.18px] border-[1.42px] border-[#181A20] gap-[7.11px] rounded-[142.22px] p_text">
            <h3 class="font-[400] text-[9.96px] leading-[11.95px] tracking-[3%]">Open House</h3>
            <h3 class="font-[700] text-[11.38px] leading-[13.65px] tracking-[4%] text-[#181A20]">September 16</h3>
            <h3 class="font-[400] text-[9.96px] leading-[11.95px] tracking-[3%]">8.AM — 2.PM</h3>
          </div>
        </div>

        <div class="flex flex-col gap-8">
          <ul class="flex justify-between items-center  font-[400] text-[14.22px] leading-[17.07px] tracking-[3%]">
            <li>beds</li>
            <li>bath</li>
            <li>garage</li>
            <li>finished sq ft</li>
          </ul>

          <ul class="flex justify-between items-center font-[500] text-[14.22px] leading-[17.07px] tracking-[3%]">
            <li>2 — 4</li>
            <li>2.5 — 3.5</li>
            <li>2</li>
            <li>1707 —1951</li>
          </ul>
          <div class="border-b-[2.42px] border-[#181A20]"></div>

          <div class="flex items-center justify-between">
            <p class="font-[500] text-[13.8px] leading-[15.36px] tracking-[3%] text-[#181A20]">555 North 400 West <br>
              Centerville, Utah 84014</p>

            <div>
              <NuxtLink to="/modern" class="button arrow flex items-center gap-5 cursor-pointer">
                <p class="text-black text-[16px] font-[600]">
                  Contact Agent
                </p>
              </NuxtLink>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>
.grid_container{
  align-items: center;
  justify-content: center;
  padding: 80px;
}



a.button {
  margin: 20px;
  font-size: 20px;
}

.arrow {
  color: #000000;
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
    color: #000000;
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
//.p_text{
//  padding: 28.88px;
//}
</style>