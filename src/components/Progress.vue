<template>
       <div class="bg-gray-50 w-[100%] h-[auto] my-16 mx-auto py-1 md:flex flex-row items-center justify-evenly md:w-[80%]">
        <p class="font-bold text-left">Progress:</p>
        <div class="w-[100%] h-[100px] my-4 flex flex-row flex-nowrap items-center justify-evenly md:w-[70%]">

            <div class="w-[33%] h-[80px] flex flex-row items-center md:w-[33%]" data-aos="fade-left">
                <div class="border-dashed border-2 p-1 border-rose-300 w-[50px] h-[50px] rounded-full md:w-[70px] md:h-[70px]">
                    <div :class="progressDetails.status >= 1 ? 'done' : 'undone'" class="rounded-full text-center w-[100%] h-[100%] md:pt-2">
                    <i class="material-symbols-outlined text-white text-center pt-1 text-[30px] md:text-[40px]">how_to_reg</i></div>
                </div>
                <p :class="progressDetails.status >= 1 ? 'done-text' : 'undone-text'" class="pl-1 text-sm md:pl-4">Enrollment</p>
            </div>
            

            <div class="w-[33%] h-[80px] flex flex-row items-center md:w-[33%]" data-aos="fade-up">
                <div class="border-dashed border-2 p-1 border-rose-300 w-[50px] h-[50px] rounded-full md:w-[70px] md:h-[70px]">
                    <div :class="progressDetails.status >= 2 ? 'done' : 'undone'" class="rounded-full text-center w-[100%] h-[100%] md:pt-2">
                    <i class="material-symbols-outlined text-white text-center pt-1 text-[30px] md:text-[40px]">payments</i></div>
                </div>
                <p :class="progressDetails.status >= 2 ? 'done-text' : 'undone-text'" class="pl-1 text-sm md:pl-4">Transfer</p>
            </div>

            <div class="w-[33%] h-[80px] flex flex-row items-center md:w-[33%]" data-aos="fade-right">
                <div class="border-dashed border-2 p-1 border-rose-300 w-[50px] h-[50px] rounded-full md:w-[70px] md:h-[70px]">
                    <div :class="progressDetails.status >= 3 ? 'done' : 'undone'" class="rounded-full text-center w-[100%] h-[100%] md:pt-2">
                    <i class="material-symbols-outlined text-white text-center pt-1 text-[30px] md:text-[40px]">paid</i></div>
                </div>
                <p :class="progressDetails.status >= 3 ? 'done-text' : 'undone-text'" class="pl-1 text-sm md:pl-4">Completed</p>
            </div>

        </div>
    </div>  
</template>

<script>
import AOS from "aos";
import "aos/dist/aos.css";

AOS.init({
  duration: 1000,
});

export default {
    name: "Progress",
    props: {
        progressDetails: Object
    },
    setup() {}

}
</script>

<style scoped>
.undone {
    @apply bg-gray-400;
}
.undone-text {
    @apply font-bold text-gray-500 ;
}
.done {
    @apply bg-[#6B9B8F];
}
.done-text {
    @apply font-bold text-gray-950;
}

</style>