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

const projects1 = ref([
    {
        title: 'Aperture',
        img: require('@/assets/img/Aperture.png'),
        subtitle: 'Photo studios, portfolio',
        url: 'https://prdz14.github.io/Aperture/'
    },
    {
        title: 'Tour-travel',
        img: './src/assets/img/Tour-travel.png',
        subtitle: 'Travel company, portfolio',
        url: 'https://prdz14.github.io/Tour-Travel/'
    },
])

const projects2 = ref([
    {
        title: 'Vue-cinema',
        img: './src/assets/img/King-kong.jpg',
        subtitle: 'Cinema, portfolio',
        url: 'https://prdz14.github.io/Vue/'
    },
    {
        title: 'Education',
        img: './src/assets/img/Education.jpg',
        subtitle: 'Education, portfolio',
        url: 'https://prdz14.github.io/Education/'
    },
])

const projects3 = ref([
    {
        title: 'Finsweet',
        img: './src/assets/img/Finsweet.jpg',
        subtitle: 'Ecology, portfolio',
        url: 'https://prdz14.github.io/Finsweet/'
    },
    {
        title: 'Solar',
        img: './src/assets/img/Solar.jpg',
        subtitle: 'Power station, portfolio',
        url: 'https://prdz14.github.io/SolarEX/'
    },
])


</script>

<style lang="scss" scoped></style>