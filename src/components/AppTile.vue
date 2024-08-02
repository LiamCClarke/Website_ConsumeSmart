<script setup>
const props = defineProps({
    icon: String,
    title: String,
    message: String
})
</script>

<template>
    <div class="tile-container">
        <div class="tile-background">
            <article class="tile-content">
                <div class="icon">{{props.icon}}</div>
                <h2>{{props.title}}</h2>
                <p>{{props.message}}</p>
            </article>
        </div>
    </div>
</template>

<style scoped>
.tile-container {
    padding: 8px;
    width: calc(100% / 3);
}

.tile-background {
    display: block;
    border: none;
    border-radius: 12px;
    height: 100%;
    background-color: var(--secondary-color);
}

.tile-content {
    display: flex;
    flex-direction: column;
    padding: 24px;
    height: 100%;
}

.icon {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-bottom: 20px;
    border-radius: 6px;
    background-color: rgba(101, 117, 133, .16);
    width: 48px;
    height: 48px;
    font-size: 24px;
}
</style>