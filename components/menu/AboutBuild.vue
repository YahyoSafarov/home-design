<template>
  <div class="container py-24">
    <div class="flex gap-10 mb-10 text-black">
      <p class="font-[500] text-[16px] leading-[19.2px] tracking-[3%]">(05)</p>
      <h1 class="font-[400] text-[50px] leading-[50px]">We Build <br>
        Community</h1>
    </div>

    <div class="flex items-center justify-end ">
      <div class="flex flex-col justify-end items-center gap-10">
        <img src="../../assets/images/Build-Image.png" alt="no image">
        <p class="font-[400] text-[32px] leading-[50px] text-[#000]">
          Ciio is a real estate development and brokerage <br>
          organization committed to developing and marketing <br>
          master-planned communities, residential lots, urban in-fill <br>
          communities, and mixed-use properties across the state <br>
          of Utah. Our foundation is built on the beliefs of <br>
          generating value through prudent land planning, <br>
          innovative architecture, and outstanding execution at the <br>
          project level.
        </p>
        <div class="">
          <p class="underline decoration-4 decoration-black text-[20px] font-[700] leading-[24px] tracking-[3%]">
            Learn More About Our Projects
          </p>
        </div>
        <div class="">
          <a class="button arrow flex items-center gap-5 cursor-pointer">
            <p class="text-black text-[16px] font-[600]">
              Download Portfolio
            </p>
          </a>
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