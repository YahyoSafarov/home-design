<template>
  <div class="container">
    <div class="section-padding gallery-section" id="gallery">
      <div class="container">
        <!-- Section Title Start -->
        <div class="text-center">
          <p class="  "> (01) Details</p>
          <h2 class="title">Our community details</h2>
        </div>
        <!-- Section Title End -->

        <div id="btncontainer" class="filter">
          <button :class="{ 'btn-active': activeFilter === 'all' }" class="btn" @click="filterGallery('all')">ALL</button>
          <button :class="{ 'btn-active': activeFilter === 'Bollywood' }" class="btn" @click="filterGallery('Bollywood')">(01) Package A</button>
          <button :class="{ 'btn-active': activeFilter === 'Hollywood' }" class="btn" @click="filterGallery('Hollywood')">(02) Package B</button>
          <button :class="{ 'btn-active': activeFilter === 'tv' }" class="btn" @click="filterGallery('tv')">(03) Package C</button>
        </div>

        <!-- Gallery Section Start -->
        <div class="grid grid-cols-1  md:grid-cols-2 xl:grid-cols-3 gap-8 mb-20 mt-28">
          <a v-for="(img, index) in filteredImages" :key="index" @click="openImage(index)">
            <div>
              <div class="overflow-hidden">
                <img :src="img.src" alt="no image" class="w-full h-[350px] object-cover transition duration-700  hover:scale-110" />
              </div>
              <div class="flex justify-between items-center gap-4 mt-2">
                <div class="flex items-center gap-1 flex-col">
                  <p class="font-[400] text-[16px] leading-[19.2px] tracking-[3%] text-black">{{img.title1}}</p>
                  <p class="font-[400] text-[12px] leading-[14.4px] tracking-[3%] text-[#7D7D7D]">{{img.mintitle1}}</p>
                </div>
                <div class=" flex flex-col gap-1">
                  <p class="font-[400] text-[16px] leading-[19.2px] tracking-[3%] text-black">{{img.title2}}</p>
                  <p class="font-[400] text-[12px] leading-[14.4px] tracking-[3%] text-[#7D7D7D]">Apartments / Starting From <br> — $1,675+ Monthly</p>
                </div>
              </div>
            </div>

          </a>
        </div>
      </div>
    </div>

    <div v-if="isModalOpen" class="openDiv">
      <img :src="images[currentImage].src" class="imgPreview" />
      <div class="butonsSection">
        <button class="prevButton" @click="prevImage">Previous</button>
        <button class="nextButton" @click="nextImage">Next</button>
      </div>
      <button class="closeBtn" @click="closeModal">Close</button>
    </div>
  </div>
</template>




<script setup>
import { ref } from 'vue';

const activeFilter = ref('all');
const currentImage = ref(0);
const isModalOpen = ref(false);

const images = ref([
  {
    id: 1,
    src: 'https://images.unsplash.com/photo-1560184897-ae75f418493e?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1yZWxhdGVkfDR8fHxlbnwwfHx8fHw%3D',
    category: 'Bollywood',
    title1: "theBEVERLY",
    mintitle1: "Salt Lake City",
    title2: "Now Leasing",
    mintitle2: "Apartments / Starting From — $1,675+ Monthly",
  },
  {
    id: 2,
    src: 'https://images.unsplash.com/photo-1605276374104-dee2a0ed3cd6?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D',
    category: 'Bollywood',
    title1: "theBEVERLY",
    mintitle1: "Salt Lake City",
    title2: "Now Leasing",
    mintitle2: "Apartments / Starting From — $1,675+ Monthly",
  },
  {
    id: 3,
    src: 'https://images.unsplash.com/photo-1628624747186-a941c476b7ef?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1yZWxhdGVkfDEwfHx8ZW58MHx8fHx8', category: 'Bollywood',
    title1: "theBEVERLY",
    mintitle1: "Salt Lake City",
    title2: "Now Leasing",
    mintitle2: "Apartments / Starting From — $1,675+ Monthly",
  },
  {
    id: 4,
    src: 'https://images.unsplash.com/photo-1600585154340-be6161a56a0c?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D',
    category: 'Bollywood',
    title1: "theBEVERLY",
    mintitle1: "Salt Lake City",
    title2: "Now Leasing",
    mintitle2: "Apartments / Starting From — $1,675+ Monthly",
  },
  { id: 5,
    src: 'https://images.unsplash.com/photo-1495433324511-bf8e92934d90?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D', category: 'Hollywood',
    title1: "theBEVERLY",
    mintitle1: "Salt Lake City",
    title2: "Now Leasing",
    mintitle2: "Apartments / Starting From — $1,675+ Monthly",
  },
  {
    id: 6,
    src: 'https://images.unsplash.com/photo-1560448204-e02f11c3d0e2?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D', category: 'Hollywood' ,
    title1: "theBEVERLY",
    mintitle1: "Salt Lake City",
    title2: "Now Leasing",
    mintitle2: "Apartments / Starting From — $1,675+ Monthly",
  },
  {
    id: 7,
    src: 'https://images.unsplash.com/photo-1465301055284-72f355cfd745?q=80&w=2003&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D', category: 'tv' ,
    title1: "theBEVERLY",
    mintitle1: "Salt Lake City",
    title2: "Now Leasing",
    mintitle2: "Apartments / Starting From — $1,675+ Monthly",
  },
  {
    id: 8,
    src: 'https://images.unsplash.com/photo-1556228453-efd6c1ff04f6?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D',
    category: 'tv',
    title1: "theBEVERLY",
    mintitle1: "Salt Lake City",
    title2: "Now Leasing",
    mintitle2: "Apartments / Starting From — $1,675+ Monthly",
  },
      {
        id: 9,
        src: 'https://plus.unsplash.com/premium_photo-1687960116689-38c34910d26f?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D',
        category: 'tv',
        title1: "theBEVERLY",
        mintitle1: "Salt Lake City",
        title2: "Now Leasing",
        mintitle2: "Apartments / Starting From — $1,675+ Monthly",
      },
      {
        id: 10,
        src: 'https://plus.unsplash.com/premium_photo-1661906314543-dd6b588f3556?q=80&w=1934&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D',
        category: 'tv',
        title1: "theBEVERLY",
        mintitle1: "Salt Lake City",
        title2: "Now Leasing",
        mintitle2: "Apartments / Starting From — $1,675+ Monthly",
      },
      {
        id: 11,
        src: 'https://images.unsplash.com/photo-1582268611958-ebfd161ef9cf?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D',
        category: 'tv',
        title1: "theBEVERLY",
        mintitle1: "Salt Lake City",
        title2: "Now Leasing",
        mintitle2: "Apartments / Starting From — $1,675+ Monthly",
      },
      {
        id: 12,
        src: 'https://images.unsplash.com/photo-1616046229478-9901c5536a45?q=80&w=1780&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D',
        category: 'tv',
        title1: "theBEVERLY",
        mintitle1: "Salt Lake City",
        title2: "Now Leasing",
        mintitle2: "Apartments / Starting From — $1,675+ Monthly",
      }
],
);

const filteredImages = computed(() => {
  if (activeFilter.value === 'all') return images.value;
  return images.value.filter(img => img.category === activeFilter.value);
});

const filterGallery = (filter) => {
  activeFilter.value = filter;
};

const openImage = (index) => {
  currentImage.value = index;
  isModalOpen.value = true;
};

const closeModal = () => {
  isModalOpen.value = false;
};

const nextImage = () => {
  currentImage.value = (currentImage.value + 1) % images.value.length;
};

const prevImage = () => {
  currentImage.value = (currentImage.value - 1 + images.value.length) % images.value.length;
};
</script>
<style scoped>
a {
  text-decoration: none;
  cursor: pointer;
  outline: 0;
}

.section-padding {
  padding-top: 80px;
}

.gallery-section {
  position: relative;
  z-index: 1;
}

.title {
  font-size: 46px;
  font-weight: 700;
  margin-bottom: 10px;
  color: #262A34;
}

.filter {
  text-align: center;
  max-width: 1050px;
  margin: auto;
}

.btn {
  padding: 10px 20px;
  margin: 5px 4px 4px 0;
  display: inline-block;
  color: #003;
  background: #eee;
  border: 1px solid #262A34;
  transition: all 0.4s;
  border-radius: 10px;
  font-size: 16px;
  font-weight: 500;
}
.btn:hover, .btn-active {
  background: #262A34;
  color: #fff;
  transform: translateY(3px);
}

.gallery {

}
.gallery a {
  display: flex;
}
.gallery img {
  width: 200px;
  height: 220px;
  object-fit: cover;
  transition: 0.3s ease-in-out;
  border-radius: 12px;
  overflow: hidden;
  margin: 10px 10px;
}

.gallery img:hover {
  transform: scale(1.1);
}

.sets .hide,
.sets .pophide {
  width: 0%;
  opacity: 0;
}

closeBtn {
  position: absolute;
  font-size: 22px;
  font-weight: 500;
  right: 25px;
  top: 25px;
  color: white;
  transition: 0.5s linear;
  padding: 8px 40px;
  border-radius: 25px;
  background: red;
  outline-offset: -6px;
  outline: 2px solid #fff;
}
.closeBtn:hover {
  cursor: pointer;
  background: white;
  color: black;
  outline: 2px solid #000;
}

.openDiv {
  width: 100%;
  height: 100vh;
  background: #000000e7;
  position: fixed;
  top: 0;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  left: 0;
  z-index: 9999;
}
.imgPreview {
  width: 70%;
  object-fit: scale-down;
  max-height: 40vw;
  height: auto;
}
.prevButton,
.nextButton {
  transition: 1s linear;
  padding: 10px 35px;
  font-size: 18px;
  border: none;
  color: white;
  background: #0005;
  border-radius: 10px;
  border: 1px solid white;
  margin: 10px;
}
.prevButton:hover,
.nextButton:hover {
  background: #fff;
  color: black;
}

/* responsive CSS Code */

@media (max-width: 1199px) {
  .section-padding {
    padding-top: 70px;
  }
}
@media (max-width: 991px) {
  .section-padding {
    padding-top: 50px;
  }
}
@media (max-width: 767px) {
  .title {
    font-size: 36px;
  }
  .gallery img {
    margin: 8px 8px;
    width: 175px;
  }
  .closeBtn {
    padding: 6px 25px;
  }
  .prevButton,
  .nextButton {
    font-size: 18px;
    padding: 8px 25px;
  }
}

@media (max-width: 540px) {
  .section-padding {
    padding-top: 30px;
  }

  .gallery img {
    margin: 8px 6px;
    width: 155px;
  }

  .closeBtn {
    font-size: 18px;
    border-radius: 15px;
  }
  .prevButton,
  .nextButton {
    font-size: 18px;
    padding: 6px 20px;
    border-radius: 10px;
    margin: 5px;
  }

  .imgPreview {
    width: 90%;
    max-height: 50vh;
    height: auto;
  }
}
</style>
