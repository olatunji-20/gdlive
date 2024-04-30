<template>
  <header class="w-[100%] h-[120px] bg-[#4D4D4D] flex flex-row justify-between items-center px-6 md:px-16">
    <router-link to="/">
      <div class="w-[170px] h-[45px] md:w-[200px] md:h-[55px]">
        <img src="/img/gdlive.svg" alt="gdlive-love" class="w-[100%] h-[100%]" />
      </div>
    </router-link>
    <div class="bg-gray-700 w-[30px] h-[30px] md:hidden"></div>
    <div class="w-[300px] h-[30px] text-center text-white hidden md:inline">
      <h5>GiveDirectly Home</h5>
    </div>
    <div class="w-[160px] h-[50px] hidden md:inline">
      <button class="bg-[#6B9B8F] w-[100%] h-[100%] rounded-md text-white hover:bg-green-900 duration-200">Give Now</button>
    </div>
  </header>
</template>

<script>
export default {

}
</script>

<style scoped>

</style>