<script setup>

const props = defineProps({
    name: String,
    text: String,
    tagline: String,
    reversed: {
        type: Boolean,
        default: false
    }
})
</script>

<template>
    <div class="hero_content" :class="{ 'hero-reversed' : reversed}">
        <div class="hero_main">
            <h1 class="name">{{props.name}}</h1>
            <p class="text">{{props.text}}</p>
            <p class="tagline">{{props.tagline}}</p>
            <div class="actions">
                <div class="action">
                    <a class="button">Get Started</a>
                </div>
            </div>
        </div>
        <div class="hero_media">
            <img class="hero_image" src="../assets/media/hero_shopping.svg" alt="bulb with brain and graduate cap">
        </div>
    </div>
</template>

<style scoped>
.hero_content {
    display: flex;
    flex-direction: row;
    justify-content: center;
    padding: 150px 0 150px;
}

.hero_main, .hero_media {
    max-width: 50%;
    width: 50%;
    max-height: var(--hero_height);
    order: 1;
}

.hero_media {
    display: flex;
    align-items: center;
    justify-content: center;
    order: 2;
}

.hero_image {
    position: absolute;
    background-color: transparent;
    height: var(--hero_height);
}

.hero-reversed {
    flex-direction: row-reverse;
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