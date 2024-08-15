<template>
    <div class="grid-wrapper">
        <div class="grid-container">
            <div class="grid-child kitchenware">
                <h1 class="title">Kitchenware</h1>
                <ul>
                    <li><router-link :to="{ name: 'Home' }">Utensils</router-link></li>
                    <li><router-link :to="{ name: 'Home' }">Pots & Pans</router-link></li>
                    <li><router-link :to="{ name: 'Home' }">Food Preperation</router-link></li>
                    <li><router-link :to="{ name: 'Home' }">Serveware</router-link></li>
                </ul>
            </div>
            <div class="grid-child clothing">
                <h1 class="title">Clothing</h1>
                <ul>
                    <li><router-link :to="{ name: 'Home' }">Coats & Jackets</router-link></li>
                    <li><router-link :to="{ name: 'Home' }">Jeans</router-link></li>
                    <li><router-link :to="{ name: 'Home' }">Belts</router-link></li>
                    <li><router-link :to="{ name: 'Home' }">Boots</router-link></li>
                </ul>
            </div>
            <div class="grid-child electronics">
                <h1 class="title">Electronics</h1>
                <ul>
                    <li><router-link :to="{ name: 'Home' }">Televisions</router-link></li>
                    <li><router-link :to="{ name: 'Home' }">Audio</router-link></li>
                    <li><router-link :to="{ name: 'Home' }">Computers</router-link></li>
                    <li><router-link :to="{ name: 'Home' }">Mobile Phones</router-link></li>
                </ul>
            </div>
            <div class="grid-child tools">
                <h1 class="title">Tools</h1>
                <ul>
                    <li><router-link :to="{ name: 'Home' }">Power Tools</router-link></li>
                    <li><router-link :to="{ name: 'Home' }">Hand Tools</router-link></li>
                    <li><router-link :to="{ name: 'Home' }">Measuring Tools</router-link></li>
                    <li><router-link :to="{ name: 'Home' }">Tool Storage</router-link></li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style scoped>
.grid-wrapper {
    display: flex;
    justify-content: center;
    width: 100%;
    padding-top: 100px;
}

.grid-container {
    display: grid;
    gap: 30px;
    grid-template-columns: auto auto;
    grid-template-rows: auto auto;
    justify-content: space-evenly;
    align-content: center;
    max-width: var(--layout-width);
}

.grid-child {
    background-color: var(--secondary-color);
    border-radius: 25px;
    width: 400px;
    height: 350px;
    padding: 25px;
    background-size: 200px;
    background-position: right bottom;
    background-repeat: no-repeat;
}

.title {
    font-weight: 600;
    font-size: 38px;
    color: var(--accent-color);
    padding-bottom: 15px;
}

li {
    margin: 10px 10px 10px;
}

li a {
    cursor: pointer;
    font-size: 20px;
    font-weight: 400;
}

.kitchenware {
    background-image: url('../assets/media/categories_cooking.svg');
}

.clothing {
    background-image: url('../assets/media/categories_clothing.svg');
}

.electronics {
    background-image: url('../assets/media/categories_electronics.svg');
}

.tools {
    background-image: url('../assets/media/categories_tools.svg');
    background-size: 225px;
}
</style>