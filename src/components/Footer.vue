<template>
<footer>
    <section id="footer-links">
        <div class="container">
            <div class="footer-cols">
                <div class="footer-lists">
                    <h2>DC COMICS</h2>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                    <h2>SHOP</h2>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                    <h2>DC</h2>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                    <h2>SITES</h2>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                </div>
            <img src="../assets/img/dc-logo-bg.png" alt="DC Logo">
            </div>
        </div>
    </section>
    <section id="sign-and-follow">
        <div class="container">
            <div class="sign-up"></div>
            <div class="socials"></div>
        </div>
    </section>
</footer>
</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style scoped>
#footer-links {
    background-image: url('../assets/img/footer-bg.jpg');
    height: 30rem;
}

.footer-cols {
    display: flex;
    justify-content: space-between;
}

.footer-cols img {
    position: relative;
    bottom: 2rem;
}

.footer-lists {
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    color: white;
    max-height: 25rem;
    margin-top: 5rem;
}
.footer-lists ul {
    list-style-type: none;
    color: grey;
}



</style>