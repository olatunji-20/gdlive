<template>
    <Navbar />
    <Hero />
    <Stories />
    <FootBar />
</template>

<script>
import Hero from '@/components/Hero.vue';
import Navbar from '../components/Navbar.vue';
import Stories from '@/components/Stories.vue';
import FootBar from '@/components/FootBar.vue';

export default {
    name: "HomePage",
    components: {
        Navbar,
        Hero,
        Stories,
        FootBar
}

}
</script>

<style>

</style>