<script setup>
import Hero from './Hero.vue'
import Features from './Features.vue'
</script>

<template>
    <div class="main-container">
        <div class="main-side-panel">

        </div>
        <div class="main-content">
            <Hero />
            <Features />
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

.main-side-panel {
}

.main-content {
    flex-basis: var(--layout-width);
    max-width: var(--layout-width);
    padding: 0 16px;
}
</style>