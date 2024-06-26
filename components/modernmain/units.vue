<template>
  <div class="container py-24">
    <div class="flex gap-10  mt-14">
      <p class="text-[16px] font-[500] leading-[19.2px] tracking-[3% ]">
        (02)
      </p>
      <p>
        Project <br>
        the Ciio
      </p>
    </div>
    <div class="mb-14">
      <h1 class="font-[400] text-[80px] leading-[100px]">
        4 Available Units
      </h1>
    </div>

    <div class="grid grid-cols-1  md:grid-cols-2 xl:grid-cols-3 gap-8">
      <div v-for="index in available" :key="index"
      >
        <div class="">

          <div class="flex flex-col gap-4">
            <img :src="index.image" class=" h-[396px] w-full" alt="no image">
            <div class="flex flex-col gap-[16px]">
              <ul class="flex justify-between">
                <li class="font-[400] text-[20px] leading-[24px] tracking-[3%]">{{index.desc1}}</li>
                <li>{{index.title1}}</li>
                <li>{{index.title2}}</li>
              </ul>
              <div class="border-b-[1px] border-[#999999]"></div>
              <ul class="flex justify-between">
                <li>{{index.desc2}}</li>
                <li>{{index.desc3}}</li>
              </ul>
              <div class="border-b-[1px] border-[#999999]"></div>
              <ul class="flex justify-between">
                <li>{{index.desc4}}</li>
                <li>{{index.number1}}</li>
              </ul>
              <div class="border-b-[1px] border-[#999999]"></div>
              <ul class="flex justify-between">
                <li>{{index.desc5}}</li>
                <li>{{index.number2}}</li>
              </ul>
              <div class="border-b-[1px] border-[#999999]"></div>
              <ul class="flex justify-between">
                <li>{{index.desc6}}</li>
                <li>{{index.number3}}</li>
              </ul>
              <div class="border-b-[1px] border-[#999999]"></div>
              <ul class="flex justify-between">
                <li>{{index.desc7}}</li>
                <li>{{index.number4}}</li>
              </ul>
              <div class="border-b-[1px] border-[#999999]"></div>
              <ul class="flex justify-between">
                <li>{{index.desc8}}</li>
                <li>{{index.number5}}</li>
              </ul>
              <div class="border-b-[1px] border-[#999999]"></div>
            </div>
          </div>
        </div>
      </div>
    </div>

  </div>
</template>

<script setup>
const available = [
  {
    id: 1,
    image: "https://images.unsplash.com/photo-1616047006789-b7af5afb8c20?q=80&w=1780&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
    desc1: "Unit #126",
    title1: "End Unit",
    title2: "$570,000",
    desc2: "Construction Status",
    desc3: "Move In Ready",
    desc4: "Bedrooms",
    number1: 6,
    desc5: "Baths",
    number2: 4.5,
    desc6: "Car Garage",
    number3: 5,
    desc7: "Square Footage",
    number4: 3000,
    desc8: "Listed by Tara Horton",
    number5: "Email | Call",
  },
  {
    id: 2,
    image: "https://images.unsplash.com/photo-1558882224-dda166733046?q=80&w=2069&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
    desc1: "Unit #126",
    title1: "End Unit",
    title2: "$570,000",
    desc2: "Construction Status",
    desc3: "Move In Ready",
    desc4: "Bedrooms",
    number1: 6,
    desc5: "Baths",
    number2: 4.5,
    desc6: "Car Garage",
    number3: 5,
    desc7: "Square Footage",
    number4: 3000,
    desc8: "Listed by Tara Horton",
    number5: "Email | Call",
  },
  {
    id: 2,
    image: "https://images.unsplash.com/photo-1551516594-56cb78394645?q=80&w=2030&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
    desc1: "Unit #126",
    title1: "End Unit",
    title2: "$570,000",
    desc2: "Construction Status",
    desc3: "Move In Ready",
    desc4: "Bedrooms",
    number1: 6,
    desc5: "Baths",
    number2: 4.5,
    desc6: "Car Garage",
    number3: 5,
    desc7: "Square Footage",
    number4: 3000,
    desc8: "Listed by Tara Horton",
    number5: "Email | Call",
  },
]
</script>

<style lang="scss" scoped>

</style>
