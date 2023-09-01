<script setup>
    import {RouterLink} from 'vue-router'
</script>

<template>
    <div>
        <RouterLink active-class="active" to="/">Home</RouterLink>
        <RouterLink active-class="active" to="/about">About</RouterLink>
    </div>
</template>

<style scoped>
    .active {
        color: blueviolet;
        font-weight: 700;
        margin: 0 10px;
        text-decoration: none;
    }
</style>