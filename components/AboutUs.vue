<template>
  <div class="bg-[#F4F1E7] h-[511px] flex items-center justify-center">
    <div class="container bg_media py-12]">
      <div class="flex justify-between items-center mb-28">
        <ul class="flex gap-10 items-center">
          <p class="text-[16px] leading-[19.2px] tracking-[3%] text-[#181A20] font-[600]">(01)</p>
          <h3 class="text-[16px] leading-[19.2px] tracking-[3%] text-[#181A20] font-[600]">About us</h3>
        </ul>
        <div>
          <a class="button arrow flex items-center gap-5 cursor-pointer">
            <p class="text-black text-[16px] font-[600]">
              Get to know us
            </p>
          </a>
        </div>
      </div>

      <div class="text_media">
        <p class=" text-[50px] leading-[50px] font-[400]">
          AChille Ciio is leading the way in creating <br>
          unique real estate for Utah residents.
        </p>
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
@media(max-width: 650px){
  bg_media{
    padding: 0px;
  }
  .text_media p{
    font-size: 40px;
    margin-top: -65px;
  }
}
</style>