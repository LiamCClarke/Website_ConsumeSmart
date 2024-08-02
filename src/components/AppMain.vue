<script setup>
import AppHero from './AppHero.vue'
import AppFeatures from './AppFeatures.vue'

const heroTop = {
    name: 'Consume Smart',
    text: 'Make Choices Quicker, Cheaper, Smarter.',
    tagline: 'Consume Smart compares essential products helping you make the smarter purchase.',
    reversed: false
}

const heroLower = {
    name: 'Test Name',
    text: 'Test Text',
    tagline: 'Test Tagline',
    reversed: true
}
</script>

<template>
    <div class="main-container">
        <div class="main-side-panel">

        </div>
        <div class="main-content">
            <AppHero :="heroTop"/>
            <AppHero :="heroLower"/>
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