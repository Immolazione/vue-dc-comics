<template>
  <header>
    <div class="container">
      <div id="header-navbar">
        <img src="../assets/img/dc-logo.png" alt="Logo DC">
        <nav>
          <ul>
            <li v-for="(link, index) in navbar" :key="index"><a href="link.url">
              {{ link.text }}
              </a></li>
          </ul>
        </nav>
      </div>
    </div>
  </header>
</template>

<script>
  export default {
    name: 'Header',
    data() {
      return {
        navbar: [
          {url: '#', text: 'CHARACTERS', active: 'false'},
          {url: '#', text: 'COMICS', active: 'false'},
          {url: '#', text: 'MOVIES', active: 'false'},
          {url: '#', text: 'TV', active: 'false'},
          {url: '#', text: 'GAMES', active: 'false'},
          {url: '#', text: 'COLLECTIBLES', active: 'false'},
          {url: '#', text: 'VIDEOS', active: 'false'},
          {url: '#', text: 'FANS', active: 'false'},
          {url: '#', text: 'NEWS', active: 'false'},
          {url: '#', text: 'SHOP', active: 'false'}
        ],
      }
    }
  }
</script>


<style scoped>
  #header-navbar{
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 8rem;
  }
  #header-navbar img {
    width: 5rem;
  }
  ul {
    display: flex;
    list-style-type: none;
  }
  ul li {
    padding: 0 0.8rem
  }
  ul li a {
    color: #000;
    text-decoration: none;
    font-size: 0.8rem;
  }
</style>
