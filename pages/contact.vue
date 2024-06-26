<template>
  <div class="bg-[#262A34]">
    <div class="container py-24">
      <div class="flex flex-col justify-center items-center">
        <h1 class="text-[96px] font-[400] leading-[106px] mb-10 text-white">Contact us</h1>
        <p class="font-[400] text-[32px] leading-[40px] text-white text-center">
          Get in touch with us, we're eager to assist you in <br> nexperiencing the unique and cutting-edge.
        </p>

        <div>
          <a class="button arrow flex items-center gap-5 cursor-pointer">
            <p class="text-white text-[16px] font-[600]">
              Support
            </p>
          </a>
        </div>
      </div>
    </div>
    <Submit />
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
  color: #ffffff;
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
    color: #ffffff;
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