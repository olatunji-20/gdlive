<template>
  <main class="bg-[#4D4D4D] w-[100%] h-[auto] flex flex-col justify-start pt-12 pb-72 md:flex-row md:justify-center md:pb-48">
    <div class="w-[100%] h-[400px] text-white px-4 md:w-[40%] py-12 md:h-[550px] md:px-8 md:pt-20">

        <div class="w-[100%] h-[130px]">
            <h1 class="text-[42px] leading-14 text-gray-50 font-bold">
                <vue-typewriter-effect :strings="'Unfiltered, Unedited Stories'" />
            </h1>
        </div>

        <p class="pt-4">We're committed to transparency and the use of our survey technology to collect and share real-time updates and stories
            in this live newsfeed.
        </p>
        <p class="font-bold pt-8 text-[#6B9B8F]" style="font-family: jackquard 24;">Learn about how we collect stories <span><i class="material-symbols-outlined relative top-2 font-bold">start</i></span></p>
    </div>
    <div class="w-[100%] h-[420px] md:w-[55%] md:h-[550px]">
        <div class="w-[400px] h-[400px] overflow-hidden m-[auto] relative flex justify-center items-center md:w-[540px] md:h-[540px]">

            <div class="zig border-2 border-green-800 bg-[#6B9B8F] rounded-full h-[10px] w-[10px] absolute"></div>

            <div class="rot3 border-2 border-green-800 bg-[#6B9B8F] rounded-full h-[15px] w-[15px] absolute"></div>
            <div class="rot border-2 border-green-800 bg-[#6B9B8F] rounded-full h-[20px] w-[20px] absolute"></div>
            <div class="rot2 border-2 border-green-800 bg-[#6B9B8F] rounded-full h-[20px] w-[20px] absolute"></div>

            <div class="border border-gray-800 w-[95%] h-[95%] rounded-full flex">
                <div class="border-2 border-gray-600 w-[75%] h-[75%] rounded-full m-[auto] flex">
                    <div class="border-4 border-gray-500 w-[60%] h-[60%] rounded-full m-[auto] flex">
                        <div class="border-2 border-orange-400 w-[40px] h-[40px] rounded-full m-[auto] bg-gray-100 p-2">
                            <img src="/img/quotes.svg" class="h-[100%] w-[100%] object-contain" />
                            <div data-aos="fade-up-left" class="w-[150px] h-[150px] relative rounded-full bottom-40 right-40">
                                <img src="/img/aaa.png" class="h-[100%] w-[100%] object-contain" />
                            </div>
                            <div data-aos="fade-up-right" class="w-[80px] h-[80px] relative rounded-full left-28 bottom-60">
                                <img src="/img/aad.png" class="h-[100%] w-[100%] object-contain" />
                            </div>
                            <div data-aos="fade-down-left" class="w-[100px] h-[100px] relative rounded-full right-40 bottom-40">
                                <img src="/img/aab.png" class="h-[100%] w-[100%] object-contain" />
                            </div>
                            <div data-aos="fade-down-right" class="w-[120px] h-[120px] relative rounded-full left-24 bottom-64">
                                <img src="/img/aac.png" class="h-[100%] w-[100%] object-contain" />
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</main>
<div class="w-[100%] h-[auto] pt-20">
    <div class="w-[80%] bg-white h-[auto] mx-[auto] relative border-b-4 bottom-36 rounded-[40px] p-8 flex flex-col md:flex-row md:bottom-36" data-aos="fade-up">
        <h2 class="text-[#6B9B8F] font-bold text-xl mx-auto my-4 md:w-[500px]">GDLive Newsfeed</h2>
        <p class="text-center md:text-left">We check in with people at each stage of the cash transfer process to see how things are going. Take a look at some of their stories as they
            appear here in real-time. Learn more about how recipients opt in to share their stories.
        </p>
    </div>
    <div class="w-[100%] h-[auto] overflow-hidden px-4 py-16 flex flex-col md:flex-row md:py-32 md:px-12">
        <div class="w-[85%] h-[auto] mx-auto text-center md:w-[35%] md:text-left">
            <h3 data-aos="slide-right" class="font-bold text-xl">Explore Recipients</h3>
            <p class="pt-6">Browse the real, unedited profiles of the recipients we serve, learn about their aspirations and follow them to stay updated as their
                 lives move forward.
            </p>
        </div>
        <div class="w-[90%] h-[30px] my-12 mx-auto flex flex-row flex-nowrap justify-between items-center md:w-[35%] relative md:top-12">
            <img data-aos="fade-down-right" src="/img/Nigeria.png" class="h-[25px] w-[30px]" />
            <img data-aos="fade-up" src="/img/USA.png" class="h-[25px] w-[30px]" />
            <img data-aos="fade-left" src="/img/Malawi.png" class="h-[25px] w-[30px]" />
            <img data-aos="slide-down" src="/img/Mozambiq.png" class="h-[25px] w-[30px]" />
            <img data-aos="slide-left" src="/img/Kenya.png" class="h-[25px] w-[30px]" />
            <img data-aos="slide-up" src="/img/Togo.png" class="h-[25px] w-[30px]" />
            <img data-aos="fade-right" src="/img/Turkey.png" class="h-[25px] w-[30px]" />
            <img data-aos="fade-down" src="/img/Liberia.png" class="h-[25px] w-[30px]" />
            <img data-aos="fade-up-left" src="/img/Yemen.png" class="h-[25px] w-[30px]" />
        </div>
    </div>
</div>
</template>

<script>

import VueTypewriterEffect from "vue-typewriter-effect";

import AOS from "aos";
import "aos/dist/aos.css";

AOS.init({
  duration: 1000,
});

export default {
    name: "Hero",
    components: {
        VueTypewriterEffect
    }

}
</script>

<style scoped>

@keyframes orbit {
    0% {
        transform: rotate(0deg) translateX(255px) rotate(0deg);
    }
    100%  {
        transform: rotate(360deg) translateX(255px) rotate(-360deg);
    }
}

@keyframes orbit2 {
    0% {
        transform: rotate(360deg) translateX(190px) rotate(-360deg);
    }
    100%  {
        transform: rotate(0deg) translateX(190px) rotate(0deg);
    }
}

@keyframes orbit3 {
    0% {
        transform: rotate(0deg) translateX(112px) rotate(0deg);
    }
    100%  {
        transform: rotate(360deg) translateX(112px) rotate(-360deg);
    }
}

@keyframes move {
    0% {
        transform: translate(-150px, 70px);
    }
    33% {
        transform: translate(100px, -230px);

    }
    66% {
        transform: translate(-250px, 150px);

    }
    100% {
        transform: translate(250px, 400px);
    }
}


.rot {
    animation: orbit 4s linear infinite;   
}
.rot2 {
    animation: orbit2 4s linear infinite;   
}
.rot3 {
    animation: orbit3 4s linear infinite;   
}
.zig  {
    animation: move 4s linear infinite;
}
</style>