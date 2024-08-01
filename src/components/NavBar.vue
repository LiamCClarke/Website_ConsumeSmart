<template>
    <header>
        <img class="nav-logo" src="../assets/media/logo1.png" alt="logo">
        <nav>
            <ul class="nav-links">
                <li><a href="#">Link 1</a></li>
                <li><a href="#">Link 2</a></li>
                <li><a href="#">Link 3</a></li>
            </ul>
        </nav>
        <a class="cta" href="#"><button>Learn More</button></a>
    </header>
</template>

<style scoped>

.container {
    display: flex;
    justify-content: space-between;
    margin: 0 auto;
    height: var(--nav-height);
}

.title {
    flex-shrink: 0;
    height: var(--nav-height);
}

.nav-bar-title {
    display: flex;
    align-items: center;
    width: 100%;
    height: var(--nav-height);
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