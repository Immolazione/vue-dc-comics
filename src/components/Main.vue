<template>
<div>
    <section id="content">
        <div class="container">
            <h1>Content goes here</h1>
        </div>
    </section>
    <section id="services-section">
        <div class="container">
            <div class="services">
                <div class="service">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="Digital Comics">
                    <h1>DIGITAL COMICS</h1>
                </div>
                <div class="service">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="Digital Comics">
                    <h1>DIGITAL COMICS</h1>
                </div>
                <div class="service">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="Digital Comics">
                    <h1>DIGITAL COMICS</h1>
                </div>
                <div class="service">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="Digital Comics">
                    <h1>DIGITAL COMICS</h1>
                </div>
                <div class="service">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="Digital Comics">
                    <h1>DIGITAL COMICS</h1>
                </div>
            </div>
        </div>
    </section>
</div>
</template>

<script>
export default {
    name: 'Main'
}
</script>

<style>
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
    line-height: 10rem;
}
</style>