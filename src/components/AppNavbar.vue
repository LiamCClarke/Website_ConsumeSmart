<script>
import { createRouter } from 'vue-router'
</script>

<template>
    <header>
        <div class="nav-container">
            <div class="nav-content">
                <h1 class="title">BIO.</h1>
                <nav>
                    <ul class="nav-links">
                        <li><a href="#">Link 1</a></li>
                        <li><a href="#">Link 2</a></li>
                        <li><a href="#">Link 3</a></li>
                    </ul>
                </nav>
                <a class="cta" href="#"><button>Learn More</button></a>
            </div>
        </div>
    </header>
</template>

<style scoped>

.nav-container {
    position: relative;
    max-width: var(--layout-width);
    margin: 0 auto;
    overflow: hidden;
}

.nav-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 12px;
}

.title {
    font-weight: 900;
    letter-spacing: 3px;
    font-size: 30px;
}

.nav-logo {
    height: var(--logo-height);
}

.content {
    flex-grow: 1;
}

.content-body {
    display: flex;
    justify-content: flex-end;
    align-items: center;
    height: var(--nav-height);
}
</style>