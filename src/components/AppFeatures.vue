<script setup>
import AppTile from './AppTile.vue'

const tileOneData = {
    icon: '⚡',
    title: 'Testing Message',
    message: 'Sequi corrupti dicta et sit molestiae accusamus placeat ratione.'
}
const tileTwoData = {
    icon: '🍕',
    title: 'Testing Message',
    message: 'Sequi corrupti dicta et sit molestiae accusamus placeat ratione.'
}
const tileThreeData = {
    icon: '📦',
    title: 'Testing Message',
    message: 'Sequi corrupti dicta et sit molestiae accusamus placeat ratione.'
}
</script>

<template>
    <div class="feature-items">
        <AppTile :="tileOneData"/>
        <AppTile :="tileTwoData"/>
        <AppTile :="tileThreeData"/>
    </div>
</template>

<style scoped>
.feature-items {
    display: flex;
    justify-content: center;
}
</style>