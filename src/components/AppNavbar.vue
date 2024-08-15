<template>
    <header>
        <div class="nav-container">
            <div class="nav-content">
                <router-link :to="{ name: 'Home' }"><h1 class="title">BIO.</h1></router-link>
                <nav>
                    <ul class="nav-links">
                        <li><router-link :to="{ name: 'Categories' }">Categories</router-link></li>
                        <li><router-link to="/test2">Test2</router-link></li>
                        <li><router-link to="/test3">Test3</router-link></li>
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
    cursor: pointer;
}

.nav-links a {
    font-weight: 600;
}

.nav-links a.router-link-exact-active {
    color: var(--accent-color);
}
</style>