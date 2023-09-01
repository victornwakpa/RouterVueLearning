<script setup>
    import {RouterLink} from "vue-router"
    import cars from "../data/cars.json"
</script>

<template>
    <div>
        <h1>Home View</h1>
        <div class="cars">
            <RouterLink :to="`./cars/${car.id}`" v-for="car in cars" :key="car.id" href="">
                {{ car.name }}
            </RouterLink>
        </div>
    </div>
</template>

<style scoped>
    .cars {
        display: flex;
    }
    .cars a {
        margin: 0 auto;
        padding: 1em;
        box-shadow: 1px 1px 10px black;
        border-radius: 0.5em;
        text-decoration: none;
    }
</style>