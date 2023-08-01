<template>
    <section class="service" id="service">
        <div class="container">
            <h2 class="service_title">service offers</h2>
            <p class="service_subtitle">Is give may shall likeness made yielding spirit a itself togeth created after sea
                is in beast beginning signs open god you're gathering ithe</p>
            <div class="service_items">
                <div class="service_item" v-for="(service, idx) in services" :key="idx">
                    <img :src="service.img" alt="">
                    <h3>{{ service.title }}</h3>
                    <p>{{ service.txt }}</p>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
import { ref } from 'vue';
import service1 from '@/assets/img/service1.png'
import service2 from '@/assets/img/service2.png'
import service3 from '@/assets/img/service3.png'
import service4 from '@/assets/img/service4.png'

const services = ref([
    {
        img: service1,
        title: 'Wp developingSSdasdas',
        txt: 'Creeping for female light years that lesser cant evening heaven isnt bearing tree',
    },
    {
        img: service2,
        title: 'vue',
        txt: 'Creeping for female light years that lesser cant evening heaven isnt bearing tree',
    },
    {
        img: service3,
        title: 'github',
        txt: 'Creeping for female light years that lesser cant evening heaven isnt bearing tree',
    },
    {
        img: service4,
        title: 'sass',
        txt: 'Creeping for female light years that lesser cant evening heaven isnt bearing tree',
    },
]);
</script>

<style lang="scss" scoped></style>