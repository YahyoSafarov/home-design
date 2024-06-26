<template>
  <div class="bg_image">
    <div class="container">
      <div class="flex items-center flex-col text-center justify-center gap-10">
        <p class="text-18px font-[500] leading-[21.6px] tracking-[3%] text-[#FAFAFA]">Building what’s next in the heart of Utah</p>
        <h1 class="font-[700] text-[116px] leading-[120px] text-[#FAFAFA]">
          Find your <br> favorite place
        </h1>
      </div>

      <div class=" flex items-center justify-center mt-14">
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

        <div class="dropdown">

          <button></button>

          <div class="options">
            <input id="radio-africa" type="radio" name="region" value="africa" checked>
            <label style="--index: 1" for="radio-africa">City</label>

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

        <div class="dropdown">

          <button></button>

          <div class="options">
            <input id="radio-africa" type="radio" name="region" value="africa" checked>
            <label style="--index: 1" for="radio-africa">Type</label>

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

        <div class="dropdown">

          <button></button>

          <div class="options">
            <input id="radio-africa" type="radio" name="region" value="africa" checked>
            <label style="--index: 1" for="radio-africa">Type</label>

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
</template>

<script setup>

</script>

<style lang="scss" scoped>
.bg_image{
  background-image:  url("../assets/images/Oval.png");
  height: 90vh;
  width: 100%;
  background-size: cover;
  background-position: center;
  padding: 0 80px;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: center;
}




$bg: #fff;
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
  color: black;
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

@media(max-width: 520px){
  .bg_image h1{
    text-align: start;
    line-height: 60px;
    font-size: 50px;
  }
  .dropdown{
    display: none;
  }
}

@media(max-width: 480px){
  .bg_image h1{
    text-align: start;
    line-height: 60px;
    font-size: 30px;
  }
}
@media(max-width: 480px){
  .bg_image h1{
    text-align: start;

    font-size: 50px;
  }
}
</style>