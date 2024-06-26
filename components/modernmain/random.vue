
<template>
  <div class="container py-12">
    <div class="flex justify-between items-center">
      <div class="flex gap-10 items-center mb-20">
        <p class="text-[16px] leading-[19.2px] tracking-[3%] font-[500]">
          (04)
        </p>
        <h1 class="text-[64px] font-[400] leading-[60px]">
          Interior <br> Finishes
        </h1>
      </div>

      <div>
        <div class="scroll-down mr-10">
          <span></span>
          <span></span>
          <span></span>
        </div>
      </div>
    </div>


    <!-- Tabs -->
    <div data-controller="tabs" data-tabs-index-value="0" class="mx-6 mt-6">
      <ul class="flex flex-co border-b border-gray-200 dark:border-gray-700">
        <li class="mr-2 bg-gray-100" data-action="click->tabs#change" data-tabs-target="tab">
          <a href="#" class="inline-block text-blue-600 hover:text-blue-700 hover:bg-gray-50 rounded-t-lg py-4 px-4 text-sm font-medium text-center">(01)  <span>Package A</span></a>
        </li>
        <li class="mr-2 inactive" data-action="click->tabs#change" data-tabs-target="tab">
          <a href="#" class="inline-block text-blue-600  hover:text-blue-700 hover:bg-gray-50 rounded-t-lg py-4 px-4 text-sm font-medium text-center">(02)  <span>Package B</span></a>
        </li>
        <li class="mr-2 inactive" data-action="click->tabs#change" data-tabs-target="tab">
          <a href="#" class="inline-block text-blue-600  hover:text-blue-700 hover:bg-gray-50 rounded-t-lg py-4 px-4 text-sm font-medium text-center">(03 )  <span>Package C</span></a>
        </li>
<!--        <li class="mr-2 inactive" data-action="click->tabs#change" data-tabs-target="tab">-->
<!--          <a href="#" class="inline-block text-blue-600 hover:text-blue-700 hover:bg-gray-50 rounded-t-lg py-4 px-4 text-sm font-medium text-center ">Contacts</a>-->
<!--        </li>-->
      </ul>
      <div class="hidden px-1 py-2" data-tabs-target="panel">
        <h3 class="text-lg font-semibold">Home Interior</h3>
        <div class="grid_container">
          <div class="gallery-container">
            <img src="https://images.unsplash.com/photo-1600585154084-4e5fe7c39198?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
            <img src="https://images.unsplash.com/photo-1600607687644-c7171b42498f?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
            <img src="https://plus.unsplash.com/premium_photo-1683917066643-346d96b85e7f?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
            <img src="https://plus.unsplash.com/premium_photo-1684445034834-c8dec93ed218?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">

          </div>
        </div>

      </div>
      <div class="hidden px-1 py-2" data-tabs-target="panel">
        <h3 class="text-lg font-semibold">
          exterior design of the house
        </h3>
        <div class="gallery-container">
          <img src="https://images.unsplash.com/photo-1513584684374-8bab748fbf90?q=80&w=2065&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
          <img src="https://images.unsplash.com/photo-1604014238170-4def1e4e6fcf?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
          <img src="https://images.unsplash.com/photo-1600047509358-9dc75507daeb?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
          <img src="https://images.unsplash.com/photo-1600563438938-a9a27216b4f5?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">

        </div>
      </div>
      <div class="hidden px-1 py-2" data-tabs-target="panel">
        <h3 class="text-lg font-semibold">
          the most beautiful tower in the world
        </h3>
        <div class="gallery-container">
          <img src="https://images.unsplash.com/photo-1533281808624-e9b07b4294ff?q=80&w=1926&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
          <img src="https://images.unsplash.com/photo-1569949381669-ecf31ae8e613?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
          <img src="https://images.unsplash.com/photo-1592241724006-f068a14cc7dc?q=80&w=2071&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">
          <img src="https://images.unsplash.com/flagged/photo-1577990233976-9f1e5eb458b3?q=80&w=1974&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="no image">

        </div>
      </div>
<!--      <div class="hidden px-1 py-2" data-tabs-target="panel">-->
<!--        <h3 class="text-lg font-semibold">Contacts</h3>-->
<!--      </div>-->
    </div>


  </div>
</template>

<script>
import { Application, Controller } from "https://unpkg.com/@hotwired/stimulus/dist/stimulus.js"
window.Stimulus = Application.start()

Stimulus.register("tabs", class extends Controller {
  static targets = [ "tab", "panel" ]
  static values = { index: Number }

  initialize() {
    this.showTab()
  }

  change(event) {
    event.preventDefault()
    this.indexValue = this.tabTargets.indexOf(event.currentTarget)
    this.showTab()
  }

  showTab() {
    this.panelTargets.forEach((el, index) => {
      index == this.indexValue ? el.classList.remove("hidden") : el.classList.add("hidden")
    })
    this.tabTargets.forEach((el, index) => {
      index == this.indexValue ? el.classList.add("bg-gray-100") : el.classList.remove("bg-gray-100")
    })
  }
})
</script>

<style lang="scss" scoped>
@keyframes gallery {
  0%{
    opacity: 1;
  }
  25%{
    opacity: 0;
  }
  50%{
    opacity: 0;
  }
  75%{
    opacity: 0;
  }
  100%{
    opacity: 1;
  }
}

.gallery-container{
  position: relative;
  max-width: 1000px;
  height: 450px;
  overflow: hidden;
  margin: 50px auto 0 auto;
  tranform: translate3d(0,0,0);
}

img {
  position: absolute;
  top: 0;
  left: 50%;
  margin-left: -50%;
  max-width: 100%;
  width: 1000px;
  height: 700px;
  object-fit: cover;
  animation-name: gallery;
  animation-duration: 10s;
  animation-iteration-count: infinite;
  animation-direction: alternate;
  animation-timimg-function: linear;
}

img:nth-of-type(1){
  z-index: 4;
}

img:nth-of-type(2){
  animation-delay: 2.5s;
  z-index: 3;
}

img:nth-of-type(3){
  animation-delay: 5s;
  z-index: 2;
}

img:nth-of-type(4){
  animation-delay: 7.5s;
  z-index: 1;
}



.scroll-down
{

}
.scroll-down span:nth-child(2)
{
  animation-delay: -0.2s;
}
.scroll-down span:nth-child(3)
{
  animation-delay: -0.4s;
}
.scroll-down span
{
  display: block;
  width: 20px;
  height: 20px;
  border-bottom: 4px solid #000;
  border-right: 4px solid #000;
  transform: rotate(45deg);
  margin: -10px;
  animation: animate 2s infinite;
}
@keyframes animate
{
  0%
  {
    opacity: 0;
    transform: rotate(45deg) translate(-20px,-20px);
  }
  50%
  {
    opacity: 1;
  }
  100%
  {
    opacity: 0;
    transform: rotate(45deg) translate(20px,20px);
  }
}

</style>
