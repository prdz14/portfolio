<template>
    <section class="portfolio" id="portfolio">
        <div class="container">
            <h2 class="portfolio_title">quality work
                Recently done project</h2>
            <div class="grid">
                <div class="portfolio_grid">
                    <div class="portfolio_grid-item" v-for="(project, idx) in  projects1 " :key="idx">
                        <img :src="project.img" alt="">
                        <div class="portfolio_grid-item-text">
                            <h3>{{ project.title }}</h3>
                            <p>{{ project.subtitle }}</p>
                            <a :href="project.url" target="_blank">Follow</a>
                        </div>
                    </div>
                </div>
                <div class="portfolio_grid">
                    <div class="portfolio_grid-item" v-for="(project, idx) in  projects2 " :key="idx">
                        <img :src="project.img" alt="">
                        <div class="portfolio_grid-item-text">
                            <h3>{{ project.title }}</h3>
                            <p>{{ project.subtitle }}</p>
                            <a :href="project.url" target="_blank">Follow</a>
                        </div>
                    </div>
                </div>
                <div class="portfolio_grid">
                    <div class="portfolio_grid-item" v-for="(project, idx) in  projects3 " :key="idx">
                        <img :src="project.img" alt="">
                        <div class="portfolio_grid-item-text">
                            <h3>{{ project.title }}</h3>
                            <p>{{ project.subtitle }}</p>
                            <a :href="project.url" target="_blank">Follow</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
import { ref } from 'vue';
import Aperture from '@/assets/img/Aperture.png';
import TourTravel from '@/assets/img/Tour-Travel.png';
import VueCinema from '@/assets/img/King-kong.jpg';
import Education from '@/assets/img/Education.jpg';
import Finsweet from '@/assets/img/Finsweet.jpg';
import Solar from '@/assets/img/Solar.jpg';

const projects1 = ref([
    {
        title: 'Aperture',
        img: Aperture,
        subtitle: 'Photo studios, portfolio',
        url: 'https://prdz14.github.io/Aperture/'
    },
    {
        title: 'Tour-travel',
        img: TourTravel,
        subtitle: 'Travel company, portfolio',
        url: 'https://prdz14.github.io/Tour-Travel/'
    },
])

const projects2 = ref([
    {
        title: 'Vue-cinema',
        img: VueCinema,
        subtitle: 'Cinema, portfolio',
        url: 'https://prdz14.github.io/Vue/'
    },
    {
        title: 'Education',
        img: Education,
        subtitle: 'Education, portfolio',
        url: 'https://prdz14.github.io/Education/'
    },
])

const projects3 = ref([
    {
        title: 'Finsweet',
        img: Finsweet,
        subtitle: 'Ecology, portfolio',
        url: 'https://prdz14.github.io/Finsweet/'
    },
    {
        title: 'Solar',
        img: Solar,
        subtitle: 'Power station, portfolio',
        url: 'https://prdz14.github.io/SolarEX/'
    },
])


</script>

<style lang="scss" scoped></style>