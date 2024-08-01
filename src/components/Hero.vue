<script setup>
import { ref } from 'vue' // ref is needed to declare reactive states

const hero_content = {
    name: '',
    text: '',
    tagline: ''
}
</script>

<template>
    <div class="hero_content">
        <!-- <div class="hero_container"> -->
            <div class="hero_main">
                <h1 class="name">Consume Smart</h1>
                <p class="text">Make Choices Quicker, Cheaper, Smarter.</p>
                <p class="tagline">Consume Smart compares essential products helping you make the smarter purchase.</p>
                <div class="actions">
                    <div class="action">
                        <a class="button">Get Started</a>
                    </div>
                </div>
            </div>
            <div class="hero_media">
                <img class="hero_image bg" src="../assets/media/hero_bulb_glow.png">
                <img class="hero_image" src="../assets/media/hero_bulb.png" alt="bulb with brain and graduate cap">
            </div>
        <!-- </div> -->
    </div>
</template>

<style scoped>
.hero_content {
    display: flex;
    flex-direction: row;
    justify-content: center;
    padding: 90px 0 90px;
}

.hero_main, .hero_media {
    max-width: 50%;
    width: 50%;
    max-height: var(--hero_height);
}

.hero_media {
    display: flex;
    align-items: center;
    justify-content: center;
}

.hero_image {
    position: absolute;
    background-color: transparent;
    height: var(--hero_height);
}

.bg {
    filter: blur(80px);
    height: calc(var(--hero_height) - 100px);
    top: 15%;
}

.name, .text {
    letter-spacing: -.4px;
    line-height: 64px;
    font-size: 56px;
    font-weight: 700;
}

.name {
    color: var(--accent-color);
}

.tagline {
    padding-top: 12px;
    line-height: 36px;
    font-size: 24px;
    font-weight: 500;
    color: #A0A0A0;
}

.actions {
    display: flex;
    align-items: center;
    padding-top: 32px;
}

.action {
    padding: 6px;
}
</style>