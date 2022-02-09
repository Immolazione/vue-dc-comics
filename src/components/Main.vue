<template>
<main>
    <section id="content">
        <div class="container">
            <h1>Content goes here</h1>
        </div>
    </section>
    <section id="services-section">
        <div class="container">
            <div class="services">
                <div class="service" v-for="(service, index) in services" :key="index">
                    <img :src="service.src" :alt="service.text">
                    <h1>{{ service.text }}</h1>
                </div>
            </div>
        </div>
    </section>
</main>
</template>

<script scoped>
export default {
    name: 'Main',
    data(){
        return {
            services: [
                {src: '../assets/img/buy-comics-digital-comics.png', url: '#', text: 'DIGITAL COMICS'},
                {src: '../assets/img/buy-comics-merchandise.png', url: '#', text: 'DC MERCHANDISE'},
                {src: '../assets/img/buy-comics-shop-locator.png', url: '#', text: 'SUBSCRIPTION'},
                {src: '../assets/img/buy-comics-shop-locator.png', url: '#', text: 'COMIC SHOP LOCATOR'},
                {src: '../assets/img/buy-dc-power-visa-svg.png', url: '#', text: 'DC POWER VISA'},
            ],
        }
    }
}
</script>

<style scoped>
#content {
    background-color: #000;
    height: 8rem;
}
#services-section {
    background-color: #0282F9;
}

.services {
    height: 10rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.service {
    color: #fff;
    display: flex;
    justify-content: center;
    align-items: center;
}

.service img {
    margin-right: 1rem;
    width: 2rem;
}

.service h1 {
    font-size: 1rem;
}

.container > h1 {
    color: #fff;
    line-height: 8rem;
}
</style>