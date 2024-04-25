<template>
  <footer data-aos="slide-down" class="text-white w-[100%] h-[auto] mt-28 mb-48 bg-[#4D4D4D] py-8 px-2 flex flex-col md:px-24 md:flex-row wrap">
    <div class="w-[100%] h-[auto]">
        <p class="my-2 text-sm">P.O. Box 3221, New York, NY 10008 info@givedirectly.org</p>
        <p class="my-2 text-sm">US: +1 646 504 4837; Kenya: +254704372011; Uganda: +256 783 705 444</p>
    </div>
    <div class="w-[100%] h-[auto]">
        <p class="my-2 text-sm">©2024 GiveDirectly, Inc, a 501(c)3 Non-Profit Privacy Policy</p>
        <div class="w-[80px] h-[auto] mt-[20px] flex flex-row justify-between">
          <div class="border-2 border-white w-[35px] h-[35px] p-1 relative top-0 rounded-full hover:cursor-pointer hover:top-2 duration-150"><img src="/img/facebook.svg" class="w-[100%] h-[100%]" /></div>
          <div class="border-2 border-white w-[35px] h-[35px] p-1 relative top-0 rounded-full hover:cursor-pointer hover:top-2 duration-150"><img src="/img/twitter.svg" class="w-[100%] h-[100%]" /></div>
        </div>
    </div>
  </footer>
</template>

<script>
import AOS from "aos";
import "aos/dist/aos.css";

AOS.init({
  duration: 1000,
});

export default {
    name: 'FootBar',
}
</script>

<style>

</style>