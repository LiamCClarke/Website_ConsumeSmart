<template>
    <div class="tile-container">
        <div class="tile-background">
            <article class="tile-content">
                <h2>Testing Header 2</h2>
                <p>This is a test of for the paragraph tag</p>
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
</style>