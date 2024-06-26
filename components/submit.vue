<template>
  <div>
    <div class=" dark:bg-dark bg-[#F4F1E7] duration-300">
      <div class="container p-10">
        <div class="grid grid-cols-1 m md:grid-cols-2 gap-4 place-items-center">
          <div>
            <div class="space-y-5 sm:p-16 pb-6">
              <div data-aos="zoom-in" class="flex items-center gap-4">
                <!-- <div className="text-primary/70 text-7xl ">
                    <h1 className="font-bold">01</h1>
                  </div> -->
                <div class="flex gap-10 mb-14">
                  <p class="font-[500] text-[16pz] leading-[19.2px] tracking-[3%] text-[#181A20]">
                    (05)
                  </p>
                  <p class="font-[500] text-[16pz] leading-[19.2px] tracking-[3%] text-[#181A20]">Did we catch your eye?</p>
                </div>
              </div>
              <div class="text_media">
                <p class="font-[400] text-[50px] leading-[50px]">
                  We enjoy connecting with new people. Reach out to us by filling out the form, sending an email, or simply giving us a call.
                </p>
              </div>
              <div>
                <div class="mt-14">
                  <p class="font-[500] text-[16px] text-[#7D7D7D] leading-[19.2px] tracking-[3%]">Phone / Email</p>
                </div>

                <div class="mt-10">
                  <p class="font-[400] text-[32px] leading-[40px]">0 00 000 000 .CITY</p>
                  <p class="font-[400] text-[32px] leading-[40px]">achille@ciio.com</p>
                </div>
              </div>
            </div>
          </div>
          <!-- {/* Image section */} -->

          <div class=" media_container grid grid-cols-2 gap-10">
            <div class="form">
              <div>
                <input type="tel" name="text" autocomplete="off" required />
                <label for="text" class="label-name">
                <span class="content-name">
                    First Name
                </span>
                </label>
              </div>

            </div>

            <div class="form">
              <div>
                <input type="text" name="text" autocomplete="off" required />
                <label for="text" class="label-name">
                <span class="content-name">
                   Last Name
                </span>
                </label>
              </div>

            </div>

            <div class="form">
              <div>
                <input type="email" name="email" autocomplete="off" required />
                <label for="email" class="label-name">
                 <span class="content-name">
                    example@gamil.com
                 </span>
                </label>
              </div>

            </div>

            <div class="form">
              <div>
                <input type="text" name="text" autocomplete="off" required />
                <label for="text" class="label-name">
                <span class="content-name">
                  Please Select
                </span>
                </label>
              </div>

            </div>

            <div class="form">
              <div>
                <input type="text" name="text" autocomplete="off" required />
                <label for="text" class="label-name">
                <span class="content-name">
                  Please Select
                </span>
                </label>
              </div>

            </div>

            <div class="form">
              <div>
                <input type="tel" name="tel" autocomplete="off" required />
                <label for=" tel" class="label-name">
                  <span class="content-name">
                    0 00 000 000
                  </span>
                </label>
              </div>

            </div>

            <div class="form">
              <div>
                <input type="text" name="text" autocomplete="off" required />
                <label for="text" class="label-name">
                <span class="content-name">
                  Please Select
                </span>
                </label>
              </div>

            </div>

            <div class="form">
              <div>
                <input type="text" name="text" autocomplete="off" required />
                <label for="text" class="label-name">
                <span class="content-name">
                  Please Select
                </span>
                </label>
              </div>

            </div>


              <div class="flex justify-center items-center mt-20">
                <a class="button arrow flex items-center gap-5 cursor-pointer">
                  <p class="text-black text-[16px] font-[600]">
                   Submit
                  </p>
                </a>
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

h1 {
  padding-bottom: 30px;
  font-weight: 900;
  font-size: 35px;
}
.form {
  width: 270px;
  position: relative;
  height: 60px;
  overflow: hidden;
}

.form input {
  width: 100%;
  height: 100%;
  color: #000;
  padding-top: 20px;
  border: none;
  background-color: #F4F1E7;
}
.form label {
  position: absolute;
  bottom: 0px;
  left: 0px;
  width: 100%;
  height: 100%;
  pointer-events: none;
  border-bottom: 1px solid #000000;
}
.form label::after {
  content: "";
  position: absolute;
  bottom: -1px;
  left: 0px;
  width: 100%;
  height: 100%;
  border-bottom: 3px solid #fce38a;
  transform: translateX(-100%);
  transition: all 0.3s ease;
}

.content-name {
  position: absolute;
  bottom: 0px;
  left: 0px;
  padding-bottom: 5px;
  transition: all 0.3s ease;
}
.form input:focus {
  outline: none;
}
.form input:focus + .label-name .content-name,
.form input:valid + .label-name .content-name {
  transform: translateY(-150%);
  font-size: 14px;
  left: 0px;
  color: #fce38a;
}
.form input:focus + .label-name::after,
.form input:valid + .label-name::after {
  transform: translateX(0%);
}


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

@media(max-width: 1200px){
  .text_media p{
    font-size: 32px !important;
  }
}

@media(max-width: 1050px){
.media_container{
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
}


@media(max-width: 995px){
  .m{
    display: flex;
    flex-direction: column;
  }
}
</style>
