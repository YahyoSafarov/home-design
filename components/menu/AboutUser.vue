<template>
  <div class="bg-[#262A34]">
    <div class="container py-24 mx-auto">
      <div class="flex gap-10 mb-10 text-white">
        <p class="font-[500] text-[16px] leading-[19.2px] tracking-[3%]">(03)</p>
        <h1 class="font-[400] text-[50px] leading-[50px]">Process Makes <br>
          perfect</h1>
      </div>

      <div>
        <div class="w-3/4 flex gap-20 transform  translate-x-[5.5%]">
          <p class="font-[400] text-[50px] leading-[50px] text-[#fff] whitespace-normal">
            Get to know the executive team, the head honchos of the Achille Ciio pack—dedicated to finding you the ideal abode to call home. (We'd give it even more, but unfortunately, that's beyond mathematical possibility.)
          </p>
        </div>

        <div class="mt-20 flex justify-end items-end mr-[70px]">
          <section>
            <div class="containerrr">
              <div class="card">
                <div class="imgbox">
                  <img src="../../assets/images/gold-haor-man.png" class="w-[470px] h-[550px] object-cover" alt="no image">
                </div>
                <div class="content">
                  <div class="contentBox">
                    <h3 class="text-black">Salim Ahmed<br><span>Founder of Achile Ciio</span></h3>
                  </div>
                </div>
              </div>
            </div>
          </section>
        </div>

        <div>
          <section class="">
            <div class="containerrr grid grid-cols-1 place-items-center md:grid-cols-2 xl:grid-cols-3 gap-8 mb-20 mt-28">
              <div v-for="index in user" :key="index"
              >
                <div class="card">
                  <div class="imgbox">
                    <img :src="index.image" class="h-[432px] w-[470px] object-cover" alt="no image">
                  </div>
                  <div class="content">
                    <div class="contentBox">
                      <h3 class="text-black">{{index.name}}<br><span>{{index.job}}</span></h3>
                    </div>
                  </div>
                </div>
              </div>

            </div>
          </section>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const user = [
  {
    id: 1,
    image: "https://t4.ftcdn.net/jpg/01/93/84/25/360_F_193842588_Oe7qZ7HejoIzyXZwaIiQBY6sjuU96nPK.jpg",
    name: "Kazi Mahbub",
    job: "CEO of Achille Ciio",
  },
  {
    id: 2,
    image: "https://t3.ftcdn.net/jpg/07/13/35/82/360_F_713358254_pM12hayFvGkMbXwU1wERawwC2Tu3Mfpy.jpg",
    name: "Fazlor Rahman",
    job: "Chief Financial Office",
  },

  {
    id: 3,
    image: "https://t3.ftcdn.net/jpg/06/32/91/32/360_F_632913287_pyej35IPG2tnAcqVxlD5QGlsJKUAYMhP.jpg",
    name: "Abdullah",
    job: "Chief Legal Officer",
  },
  {
    id: 4,
    image: "https://www.simplilearn.com/ice9/free_resources_article_thumb/Full_stack_developer_salary.jpg",
    name: "Samim Ahmed",
    job: "VP of Design & Architecture",
  },
  {
    id: 5,
    image: "https://www.shutterstock.com/image-photo/portrait-happy-caucasian-man-smiling-260nw-1859707081.jpg",
    name: "Maruf Ahmed",
    job: "VP of Operations",
  },
  {
    id: 6,
    image: "https://t3.ftcdn.net/jpg/06/36/06/20/360_F_636062005_PhSsuSM8tADiv7D86HxuEYtYOy5NLZjn.jpg",
    name: "Dildar Khan",
    job: "VP of Commercial Operations",
  },

]
</script>

<style lang="scss" scoped>

.containerrr .card {
  position: relative;
  width: 400px;
  height: 400px;
  margin: 20px;
  overflow: hidden;
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
  border-radius: 15px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.containerrr .card .content {
  position: absolute;
  bottom: -160px;
  width: 100%;
  height: 160px;
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 10;
  flex-direction: column;
  backdrop-filter: blur(15px);
  box-shadow: 0 -10 10px rgba(0, 0, 0, 0.1);
  border: 1px solid rgba(255, 255, 255, 0.2);
  transition: bottom 0.5s;
  transition-delay: 0.8s;
}
.containerrr .card:hover .content {
  bottom: 0px;
  transition-delay: 0s;
}
.containerrr .card .content .contentBox h3 {
  color: #ffffff;
  text-transform: uppercase;
  letter-spacing: 2px;
  font-weight: 500;
  font-size: 18px;
  text-align: center;
  margin: 20px 0 15px;
  line-height: 1.1em;
  transition: 0.5s;
  opacity: 0;
  transform: translate(20px, 30px);
  transition-delay: 0.6s;
}
.containerrr .card:hover .content .contentBox h3 {
  opacity: 1;
  transform: translateY(0px);
}
.containerrr .card .content .contentBox h3 span {
  font-size: 12px;
  font-weight: 300;
  text-transform: initial;
}
.containerrr .card .content .sci {
  position: relative;
  bottom: 10px;
  display: flex;
}
.containerrr .card .content .sci li {
  list-style: none;
  margin: 0 10px;
  transform: translateY(40px);
  transition: 0.5s;
  opacity: 0;
  transition-delay: calc(0.2s * var(--i));
}
.containerrr .card:hover .content .sci li {
  transform: translateY(0px);
  opacity: 1;
}

.containerrr .card .content .sci li a {
  color: #fff;
  font-size: 24px;
}

</style>