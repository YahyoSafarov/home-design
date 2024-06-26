<template>
  <div>
    <div class=" dark:bg-dark bg duration-300">
      <div class="container py-24">
        <div class=" container flex justify-between mb-10">
          <div class="flex gap-8">
            <p class="font-[500] text-black text-[16px]">(01)</p>
            <h1 class="font-[400] text-[#7d7d7d] sm:text-[16px] leading-[19.2px] tracking-[3%]  mb-4">
              Project <br>
              <span class="font-[500] text-black">the Ciio</span>
            </h1>
          </div>
          <h3 class="mr-[600px] font-[500] text-black text-[16px]">Neighborhood <br>
           <span class="font-[400] text-[#7d7d7d] sm:text-[16px] leading-[19.2px] tracking-[3%] ">Centerville</span> </h3>
        </div>
        <div class="grid grid-cols-1 m md:grid-cols-2 gap-4 place-items-center">
          <div>
            <div class="space-y-5 sm:p-16 pb-6">
              <div data-aos="zoom-in" class="flex items-center gap-4">
              </div>

              <div>
                <p class="font-[400] text-[32px] leading-[40px] mb-20">
                  the Ciio merges cutting-edge design with suburban comfort, delivering a unique blend of modernity and community in established neighborhoods.
                </p>
              </div>
              <div>
                <div class="flex flex-col gap-4">
                  <div class="flex flex-col gap-4">
                    <p>Starting Form</p>
                    <h2 class="font-[400] text-[50px] leading-[50px] text-black">Low $500K's</h2>
                  </div>
                  <div>
                    <div class="flex gap-8 items-center">
                      <p>(01)</p>
                      <a class="button arrow flex items-center gap-5 cursor-pointer">
                        <p class="text-black text-[16px] font-[600]">
                          Calculate your Costs
                        </p>
                      </a>
                    </div>

                    <div class="border border-blas w-[270px]"></div>

                    <div class="flex gap-8 items-center">
                      <p>(02)</p>
                      <a class="button arrow flex items-center gap-5 cursor-pointer">
                        <p class="text-black text-[16px] font-[600]">
                          Calculate your Costs
                        </p>
                      </a>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>

          <div>
            <img src="../../assets/images/neighboor-home.png" alt="" class="z-40" />

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
  margin: 10px;
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
@media(max-width: 995px){
  .m{
    display: flex;
    flex-direction: column;
  }
}
</style>




<!--<template>-->
<!--  <div>-->
<!--    &lt;!&ndash; Tabs &ndash;&gt;-->
<!--    <div data-controller="tabs" data-tabs-index-value="0" class="mx-6 mt-6">-->
<!--      <ul class="flex flex-co border-b border-gray-200 dark:border-gray-700">-->
<!--        <li class="mr-2 bg-gray-100" data-action="click->tabs#change" data-tabs-target="tab">-->
<!--          <a href="#" class="inline-block text-blue-600 hover:text-blue-700 hover:bg-gray-50 rounded-t-lg py-4 px-4 text-sm font-medium text-center">Profile</a>-->
<!--        </li>-->
<!--        <li class="mr-2 inactive" data-action="click->tabs#change" data-tabs-target="tab">-->
<!--          <a href="#" class="inline-block text-blue-600  hover:text-blue-700 hover:bg-gray-50 rounded-t-lg py-4 px-4 text-sm font-medium text-center">Dashboard</a>-->
<!--        </li>-->
<!--        <li class="mr-2 inactive" data-action="click->tabs#change" data-tabs-target="tab">-->
<!--          <a href="#" class="inline-block text-blue-600  hover:text-blue-700 hover:bg-gray-50 rounded-t-lg py-4 px-4 text-sm font-medium text-center">Settings</a>-->
<!--        </li>-->
<!--        <li class="mr-2 inactive" data-action="click->tabs#change" data-tabs-target="tab">-->
<!--          <a href="#" class="inline-block text-blue-600 hover:text-blue-700 hover:bg-gray-50 rounded-t-lg py-4 px-4 text-sm font-medium text-center ">Contacts</a>-->
<!--        </li>-->
<!--      </ul>-->
<!--      <div class="hidden px-1 py-2" data-tabs-target="panel">-->
<!--        <h3 class="text-lg font-semibold">Profile</h3>-->
<!--      </div>-->
<!--      <div class="hidden px-1 py-2" data-tabs-target="panel">-->
<!--        <h3 class="text-lg font-semibold">Dashboard</h3>-->
<!--      </div>-->
<!--      <div class="hidden px-1 py-2" data-tabs-target="panel">-->
<!--        <h3 class="text-lg font-semibold">Settings</h3>-->
<!--      </div>-->
<!--      <div class="hidden px-1 py-2" data-tabs-target="panel">-->
<!--        <h3 class="text-lg font-semibold">Contacts</h3>-->
<!--      </div>-->
<!--    </div>-->


<!--  </div>-->
<!--</template>-->

<!--<script>-->
<!--import { Application, Controller } from "https://unpkg.com/@hotwired/stimulus/dist/stimulus.js"-->
<!--window.Stimulus = Application.start()-->

<!--Stimulus.register("tabs", class extends Controller {-->
<!--  static targets = [ "tab", "panel" ]-->
<!--  static values = { index: Number }-->

<!--  initialize() {-->
<!--    this.showTab()-->
<!--  }-->

<!--  change(event) {-->
<!--    event.preventDefault()-->
<!--    this.indexValue = this.tabTargets.indexOf(event.currentTarget)-->
<!--    this.showTab()-->
<!--  }-->

<!--  showTab() {-->
<!--    this.panelTargets.forEach((el, index) => {-->
<!--      index == this.indexValue ? el.classList.remove("hidden") : el.classList.add("hidden")-->
<!--    })-->
<!--    this.tabTargets.forEach((el, index) => {-->
<!--      index == this.indexValue ? el.classList.add("bg-gray-100") : el.classList.remove("bg-gray-100")-->
<!--    })-->
<!--  }-->
<!--})-->
<!--</script>-->

<!--<style lang="scss" scoped>-->

<!--</style>-->






