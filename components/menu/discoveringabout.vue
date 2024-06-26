<template>
  <div class="container py-24">
    <div>
      <div class="flex gap-24 items-center text-[16px] leading-[19.2px] tracking-[3%]">
        <h2>
          September
        </h2>
        <h2>theLANE</h2>
      </div>


        <div class="flex flex-col gap-14">

          <div v-for="index in house" :key="index"
          >
              <div class="grid grid-cols-1 md:grid-cols-2 gap-20 transform  translate-x-[3%] place-items-center">
                <div class=" flex gap-20 justify-center">
                  <div class="flex flex-col">
                    <h1 class="font-[400] text-[64px] leading-[50px] mb-14">{{index.number}}</h1>
                    <p class="text-[14px] font-[400] leading-[16.8px] tracking-[3%]">{{index.clock}}</p>
                  </div>


                  <div>
                    <div class="flex mb-14 gap-4">
                      <h1 class="font-[400] text-[64px] leading-[50px]">
                        {{index.title1}}
                      </h1>
                      <span class="font-[400] text-[32px] leading-[40px]">{{index.title2}}</span>


                    </div>
                    <div class="flex gap-8 text-[14px] font-[400] leading-[16.8px] tracking-[3%]">
                      <div class="">
                        <p class="whitespace-normal">
                          {{index.desc1}}
                        </p>
                      </div>

                      <div class="w-3/4 ...">
                        <p class="whitespace-normal">
                          {{index.desc2}}
                        </p>
                      </div>

                    </div>
                  </div>
                </div>

                <div>
                  <img :src="index.images" class="w-[352px] h-[331px] object-cover" alt="no image">
                </div>
              </div>
            <div class="border-b-[2px] border-[#999999] py-4"></div>
          </div>
        </div>
    </div>
  </div>
</template>

<script setup>
const house = [
  {
    id: 1,
    number: 10,
    clock: "11am - 1pm",
    title1: "Sales Launch",
    title2: "/theLANE",
    desc1: "644 W Porter Lance\n" +
        "Centerville, Utah 84014",
    desc2: "Join us for the sales launch at theALICE. 22 For Sale Townhomes in\n" +
        "Layton, Utah. This event will be held on site. We highly recommend\n" +
        "attending if you plan to purchase a home in this community.",
    images: "https://images.unsplash.com/photo-1416331108676-a22ccb276e35?q=80&w=2067&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
  },

  {
    id: 2,
    number: 10,
    clock: "11am - 1pm",
    title1: "Sales Launch",
    title2: "/theLANE",
    desc1: "644 W Porter Lance\n" +
        "Centerville, Utah 84014",
    desc2: "Join us for the sales launch at theALICE. 22 For Sale Townhomes in\n" +
        "Layton, Utah. This event will be held on site. We highly recommend\n" +
        "attending if you plan to purchase a home in this community.",
    images: "https://images.unsplash.com/photo-1600195075976-6c1d19c956d5?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
  },

  {
    id: 3,
    number: 10,
    clock: "11am - 1pm",
    title1: "Sales Launch",
    title2: "/theLANE",
    desc1: "644 W Porter Lance\n" +
        "Centerville, Utah 84014",
    desc2: "Join us for the sales launch at theALICE. 22 For Sale Townhomes in\n" +
        "Layton, Utah. This event will be held on site. We highly recommend\n" +
        "attending if you plan to purchase a home in this community.",
    images: "https://images.unsplash.com/photo-1494526585095-c41746248156?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
  },

  {
    id: 4,
    number: 10,
    clock: "11am - 1pm",
    title1: "Sales Launch",
    title2: "/theLANE",
    desc1: "644 W Porter Lance\n" +
        "Centerville, Utah 84014",
    desc2: "Join us for the sales launch at theALICE. 22 For Sale Townhomes in\n" +
        "Layton, Utah. This event will be held on site. We highly recommend\n" +
        "attending if you plan to purchase a home in this community.",
    images: "https://plus.unsplash.com/premium_photo-1671358689953-ee06a6671fce?q=80&w=1932&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
  },

  {
    id: 5,
    number: 10,
    clock: "11am - 1pm",
    title1: "Sales Launch",
    title2: "/theLANE",
    desc1: "644 W Porter Lance\n" +
        "Centerville, Utah 84014",
    desc2: "Join us for the sales launch at theALICE. 22 For Sale Townhomes in\n" +
        "Layton, Utah. This event will be held on site. We highly recommend\n" +
        "attending if you plan to purchase a home in this community.",
    images: "https://images.unsplash.com/photo-1626222628055-fb92dd194160?q=80&w=1974&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
  },
]
</script>

<style lang="scss" scoped>

</style>