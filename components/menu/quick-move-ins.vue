<template>
  <div class="bg-[#F4F1E7]">
    <div class="container py-44 pb-12 mx-auto h-[600px]">
      <div class="flex items-center gap-28 container">
        <div>
          <h1 class="font-[400] text-[80px] leading-[100px] ">
            Al is eager and ready <br> to move in.
          </h1>
          <p class="font-[400] leading-[24px] text-[20px] tracking-[3%] text-[#7D7D7D] mt-10">
            Enjoy the benefits of new construction without the delay by exploring <br> our available quick move-in homes below.
          </p>
        </div>

        <div>
          <div class="dropdown">

            <button></button>

            <div class="options">
              <input id="radio-africa" type="radio" name="region" value="africa" checked>
              <label style="--index: 1" for="radio-africa">Community</label>

              <input id="radio-asia" type="radio" name="region" value="asia">
              <label style="--index: 2" for="radio-asia">Asia</label>

              <input id="radio-australia" type="radio" name="region" value="australia">
              <label style="--index: 3" for="radio-australia">Australia</label>

              <input id="radio-europe" type="radio" name="region" value="europe">
              <label style="--index: 4" for="radio-europe">Europe</label>


            </div>

            <svg viewBox="0 0 24 24">
              <path d="M7.41 8.59L12 13.17l4.59-4.58L18 10l-6 6-6-6 1.41-1.41z"></path>
            </svg>

          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>


$bg: #F4F1E7;
$bg-hover: hsl(0, 0%, 84%);
$padding: 18px 21px;

* {
  box-sizing: border-box;
}
.dropdown {
  position: relative;
  box-sizing: content-box;
  width: 210px;
  height: 1em;
  padding: $padding;
  background: $bg;
  color: #000;
  box-shadow: 0 4px 4px rgba(0, 0, 0, 0.1);

  &:hover svg {
    transform: scale(1.1);
  }

  button {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    z-index: 3;
    border: none;
    outline: none;
    background: none;
    cursor: pointer;

    &:focus {
      & ~ svg {
        transform: rotate(-180deg);
        //transform: scaleY(-1);
      }
    }
  }

  .options {
    position: absolute;
    width: 100%;
    top: 0;
    left: 0;

  }

  input {
    display: none;


    &:checked + label {
      display: block;
      z-index: 2;
      font-weight: 600;
      transform: none !important;

    }
  }

  label {
    position: absolute;
    width: 100%;
    z-index: 1;
    padding: $padding;
    line-height: 1;
    background-color: $bg;
    cursor: pointer;
    transition: background-color 0.2s, transform 0.2s ease ;

    &:hover {
      background-color: $bg-hover;
      color: black;
    }
  }

  button:focus + .options input:not(:checked) + label, .options label:active, .options label:active ~ label {
    transform: translateY(calc(var(--index) * 100%));
  }

  button:focus + .options input:checked + label ~ label, .options input:checked ~ label:active, .options input:checked ~ label:active ~ label {
    transform: translateY(calc((var(--index) - 1) * 100%));
  }

  svg {
    position: absolute;
    width: 21px;
    top: 25%;
    right: 14px;
    z-index: 2;
    fill: currentColor;
    transition: transform 0.1s;
  }
}
</style>