<template>
<main>
    <section id="jumbotron">
    </section>
    <section id="content">
        <div class="container">
            <div id="current-series">CURRENT SERIES</div>
            <div class="card-box">
                <div class="card" v-for="(card, index) in cardDetails" :key="index">
                    <img :src="card.thumb" :alt="card.series">
                    <h4>{{ card.series }}</h4>
                </div>
            </div>
            <div class="load-more">
                <button type="button">LOAD MORE</button>
            </div>
        </div>
    </section>
    <section id="services-section">
        <div class="container">
            <div class="services">
                <div class="service" v-for="(service, index) in services" :key="index">
                    <img :src="require(`../assets/img/${service.src}`)" :alt="service.text">
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
                {src: 'buy-comics-digital-comics.png', url: '#', text: 'DIGITAL COMICS'},
                {src: 'buy-comics-merchandise.png', url: '#', text: 'DC MERCHANDISE'},
                {src: 'buy-comics-subscriptions.png', url: '#', text: 'SUBSCRIPTION'},
                {src: 'buy-comics-shop-locator.png', url: '#', text: 'COMIC SHOP LOCATOR'},
                {src: 'buy-dc-power-visa.svg', url: '#', text: 'DC POWER VISA'},
            ],

            cardDetails: [
                {thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                price: "$19.99",
                series: "Action Comics",
                type: "comic book"},

                {thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                price: "$3.99",
                series: "American Vampire 1976",
                type: "comic book"},

                {thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                price: "$16.99",
                series: "Aquaman",
                type: "graphic novel"},

                {thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                price: "$2.99",
                series: "Batgirl",
                type: "comic book"},

                {thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                price: "$3.99",
                series: "Batman",
                type: "comic book"},

                {thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                price: "$2.99",
                series: "Batman Beyond",
                type: "comic book"},

                {thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                price: "$3.99",
                series: "Batman/Superman",
                type: "comic book"},

                {thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                price: "$4.99",
                series: "Batman/Superman Annual",
                type: "comic book"},
            
                {thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                price: "$5.99",
                series: "Batman: The Joker War Zone",
                type: "comic book"},

                {thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                price: "$6.99",
                series: "Batman: Three Jokers",
                type: "comic book"},

                {thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                price: "$4.99",
                series: "Batman: White Knight Presents: Harley Quinn",
                type: "comic book"},

                {thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                price: "$16.99",
                series: "Catwoman",
                type: "graphic novel"}
            ]
        }
    }
}
</script>

<style scoped>
#jumbotron {
    background-image: url(../assets/img/jumbotron.jpg);
    height: 25rem;
}
#current-series{
    color: #fff;
    padding: 1rem;
    background-color: #0282F9;
    display: inline-block;
    position: relative;
    bottom: 1.5rem;
}
.card-box{
    display: flex;
    flex-wrap: wrap;
    
}
.card{
    margin: 0 2rem;
}
.card img{
    object-fit: cover;
    object-position: top;
    height: 10rem;
    width: 10rem;
}
.card h4{
    color: #fff;
    text-transform: uppercase;
    max-width: 10rem;
    font-size: 0.8rem;
}
.load-more{
    display: flex;
    justify-content: center;
}
.load-more button {
    background-color: #0282F9;
    border: 0;
    color: #fff;
    padding: 1rem 2rem;
    margin: 2rem;
}
#content {
    background-color: #000;
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
    height: 3rem;
}

.service h1 {
    font-size: 1rem;
}

.container > h1 {
    color: #fff;
    line-height: 8rem;
}
</style>