<template>
  <header>
    <div class="container">
      <div id="header-navbar">
        <img src="../assets/img/dc-logo.png" alt="Logo DC">
        <nav>
          <ul>
            <li><a href="#">CHARACTERS</a></li>
            <li><a href="#">COMICS</a></li>
            <li><a href="#">MOVIES</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">GAMES</a></li>
            <li><a href="#">COLLECTIBLES</a></li>
            <li><a href="#">VIDEOS</a></li>
            <li><a href="#">FANS</a></li>
            <li><a href="#">NEWS</a></li>
            <li><a href="#">SHOP</a></li>
          </ul>
        </nav>
      </div>
    </div>
  </header>
</template>

<script>
  export default {
    name: 'Header',
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
