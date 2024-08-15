<script setup>
import AppHero from '../components/AppHero.vue'
import AppFeatures from '../components/AppFeatures.vue'

const heroTop = {
    name: 'Buy It Once.',
    text: 'Make Smarter, Quicker, and More Affordable Choices.',
    tagline: 'Buy It Once helps you compare and find the most durable and cost-effective products, using community-driven insights to ensure every purchase is a smart one.',
    reversed: false
}
</script>

<template>
    <div class="main-container">
        <div class="main-side-panel">

        </div>
        <div class="main-content">
            <AppHero v-bind="heroTop"/>
            <AppFeatures />
        </div>
        <div class="main-side-panel">

        </div>
    </div>
</template>

<style scoped>
.main-container {
    display: flex;
    flex-direction: row;
    justify-content: center;
    width: 100%;
}

.main-content {
    flex-basis: var(--layout-width);
    max-width: var(--layout-width);
    padding: 0 16px;
}
</style>