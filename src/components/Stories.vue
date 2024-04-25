<template>
    <main class="bg-gray-100 w-[100%] h-[auto] py-12 px-4 md:p-32">
        <div class="w-[100%] h-[40px] flex flex-row no-wrap justify-between items-center">
            <div class="rounded-md w-[auto] h-[auto] p-0.5 bg-gray-50 flex flex-row flex-nowrap">
                <div class="w-[30px] h-[30px] cursor-pointer text-center pt-0.5"><i class="material-symbols-outlined font-bold">search</i></div>
                <div class="h-[30px] w-[350px] ml-2">
                    <input placeholder="search name, country or region" class="bg-transparent w-[100%] h-[100%] text-xs indent-2" />
                </div>
            </div> 
            <div class="bg-green-400 w-[100px] h-[30px] text-center">
                <img src="/img/gdlive.svg" class="w-[100%] h-[100%]" />
            </div>
        </div>
        <div class="w-[100%] h-[auto] mt-12" data-aos="fade-out">
            <EachStory />
        </div>
        <div class="w-[100%] h-[50px] mx-auto my-12 text-center md:w-[250px]">
            <button class="bg-[#095845] w-[100%] h-[100%] rounded-md text-white hover:bg-green-700 duration-200">Load More</button>
        </div>
    </main>
</template>

<script>
import EachStory from '../components/EachStory.vue';

import AOS from "aos";
import "aos/dist/aos.css";

AOS.init({
  duration: 1000,
});

export default {
    name: 'Stories',
    setup() {

        return {

        }
    },
    components: {
        EachStory,
    }

}
</script>

<style>

</style>