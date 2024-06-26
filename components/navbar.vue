<template>
  <div>
    <nav class="nav h-[94px] flex flex-wrap items-center justify-between px-20">
      <div class="flex flex-no-shrink items-center mr-6 py-3 text-grey-darkest">
        <NuxtLink to="/">
          <img src="../assets/images/Achille%20Ciio%20logo.svg  " class="w-[105px] h-[16px]" alt="no image">
        </NuxtLink>
      </div>

      <input class="menu-btn hidden" type="checkbox" id="menu-btn">
      <label class="menu-icon block cursor-pointer md:hidden px-2 py-4 relative transition duration-500 select-none" for="menu-btn">
        <span class="navicon bg-grey-darkest flex items-center relative"></span>
      </label>

      <ul class="menu border-b md:border-none flex justify-end list-reset m-0 w-full md:w-auto">
        <li class="border-t md:border-none">
          <NuxtLink to="/menumain" class="block md:inline-block px-4 py-3 no-underline text-grey-darkest hover:text-grey-darker font-bold">Search</NuxtLink>
        </li>

        <li class="border-t md:border-none">
          <NuxtLink to="/mainmenu" class="block md:inline-block px-4 py-3 no-underline text-grey-darkest hover:text-grey-darker">Communities</NuxtLink>
        </li>

        <li class="border-t md:border-none">
          <NuxtLink to="/Quick-Move-ins-menu" class="block md:inline-block px-4 py-3 no-underline text-grey-darkest hover:text-grey-darker">Quick Move-ins</NuxtLink>
        </li>

        <li class="border-t md:border-none">
          <NuxtLink to="/discovering" class="block md:inline-block px-4 py-3 no-underline text-grey-darkest hover:text-grey-darker">Open Houses</NuxtLink>
        </li>

        <li class="border-t md:border-none">
          <NuxtLink to="/about" class="block md:inline-block px-4 py-3 no-underline text-grey-darkest hover:text-grey-darker">About</NuxtLink>
        </li>

      </ul>

      <ul class="menu border-b md:border-none flex justify-end list-reset m-0 w-full md:w-auto">
        <li class="border-t md:border-none">
          <a href="/blog/" class="block md:inline-block px-4 py-3 no-underline text-grey-darkest hover:text-grey-darker">0 00 000 000 .CITY</a>
        </li>
        <li class="border-t md:border-none">
          <NuxtLink to="/contact" class="block md:inline-block px-4 py-3 no-underline text-grey-darkest hover:text-grey-darker">Contact</NuxtLink>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script setup>

</script>

<style  scoped>
.nav{
  position: relative;
  z-index: 9999;
}


@media (max-width: 767px) {
  .navicon {
    width: 1.125em;
    height: .125em;
  }
  .menu{
    transition: 0.54s ease;
    background: #ffffff;
  }

  .navicon::before,
  .navicon::after {
    display: block;
    position: absolute;
    width: 100%;
    height: 100%;
    transition: all .4s ease-out;
    content: '';
    background: #3D4852;
  }

  .navicon::before {
    top: 5px;
  }

  .navicon::after {
    top: -5px;
  }

  .menu-btn:not(:checked) ~ .menu {
    display: none;
  }

  .menu-btn:checked ~ .menu {
    display: block;
    transition: 0.5s ease;
  }

  .menu-btn:checked ~ .menu-icon .navicon {
    background: #ffffff;
    transition: 0.5s ease;
  }

  .menu-btn:checked ~ .menu-icon .navicon::before {
    transform: rotate(-45deg);
  }

  .menu-btn:checked ~ .menu-icon .navicon::after {
    transform: rotate(45deg);
  }

  .menu-btn:checked ~ .menu-icon .navicon::before,
  .menu-btn:checked ~ .menu-icon .navicon::after {
    top: 0;
  }
}

</style>