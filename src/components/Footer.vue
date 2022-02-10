<template>
<footer>
    <section id="footer-links">
        <div class="container">
            <div class="footer-cols">
                <div class="footer-lists" v-for="(link, index) in footerLinks" :key="index">
                    <h2>{{ link.title }}</h2>
                    <ul>
                        <li><a href="">{{  }}</a></li>
                    </ul>
                </div>
                <img src="../assets/img/dc-logo-bg.png" alt="DC Logo">
            </div>
        </div>
    </section>
    <section id="sign-and-follow">
        <div class="container">
            <div id="sign-and-follow-cols">
                <button type="button" class="sign-up">SIGN-UP NOW!</button>
                <div class="socials">
                    <h2>FOLLOW US</h2>
                    <img src="../assets/img/footer-facebook.png" alt="Follow">
                    <img src="../assets/img/footer-twitter.png" alt="Follow">
                    <img src="../assets/img/footer-youtube.png" alt="Follow">
                    <img src="../assets/img/footer-pinterest.png" alt="Follow">
                    <img src="../assets/img/footer-periscope.png" alt="Follow">
                </div>
            </div>
        </div>
    </section>
</footer>
</template>

<script>
export default {
    name: 'Footer',
    data(){
        return{
            footerLinks: [
                {
                    title: 'DC COMICS',
                    text: [
                    {url: '#', text: 'Characters'},
                    {url: '#', text: 'Comics'},
                    {url: '#', text: 'Movies'},
                    {url: '#', text: 'TV'},
                    {url: '#', text: 'Games'},
                    {url: '#', text: 'Videos'},
                    {url: '#', text: 'News'},
                    ]
                },
                {
                    title: 'SHOP',
                    text: [
                        {url: '#', text: 'Shop DC'},
                        {url: '#', text: 'Shop DC Collectibles'},
                    ]
                },
                {
                    title: 'DC',
                    text: [
                        {url: '#', text: 'Term Of Use'},
                        {url: '#', text: 'Privacy Policy (New)'},
                        {url: '#', text: 'Ad Choices'},
                        {url: '#', text: 'Advertising'},
                        {url: '#', text: 'Jobs'},
                        {url: '#', text: 'Subscriptions'},
                        {url: '#', text: 'Talent Workshops'},
                        {url: '#', text: 'CPSC Certificates'},
                        {url: '#', text: 'Ratings'},
                        {url: '#', text: 'Shop Help'},
                        {url: '#', text: 'Contact Us'},
                    ],
                },
                {
                    title: 'SITES',
                    text: [
                        {url: '#', text: 'DC'},
                        {url: '#', text: 'MAD Magazine'},
                        {url: '#', text: 'DC Kids'},
                        {url: '#', text: 'DC Universe'},
                        {url: '#', text: 'DC Power Visa'},
                    ],
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/_vars.scss";

#footer-links {
    background-image: url('../assets/img/footer-bg.jpg');
    height: 30rem;
    background-size: cover;
    background-repeat: no-repeat;
}

.footer-cols {
    display: flex;
    justify-content: space-between;
    img {
    position: relative;
    bottom: 2rem;
    }
}

.footer-lists {
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    color: white;
    max-height: 25rem;
    margin-top: 5rem;
    ul {
        list-style-type: none;
        li a {
        text-decoration: none;
        color: grey;
        }
    }
}

#sign-and-follow {
    height: 5rem;
    background-color: #303030;
    display: flex;
    align-items: center;
    position: relative;
    z-index: 1;
    .sign-up {
    background-color: #303030;
    color: white;
    border: 2px solid $main-color;
    padding: 0.8rem;
    }
}

#sign-and-follow-cols {
    display: flex;
    justify-content: space-between;
        .socials {
        display: flex;
        flex-grow: 1;
        justify-content: flex-end;
        align-items: center;
        * {
            margin-left: 1rem;
        }
        h2 {
            color: #0282F9;
        }
    }
}
</style>