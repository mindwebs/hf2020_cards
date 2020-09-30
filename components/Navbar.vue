<template>
  <nav>
    <div class="container">
      <h1>HF2020 Cards</h1>
      <ul>
        <li><a href="/">Home</a></li>
        <li><a href="https://hacktoberfest.digitalocean.com/">About Hacktoberfest</a></li>
      </ul>
    </div>
  </nav>
</template>

<style scoped>
  nav {
    padding: 20px 0;
    background-color: #eee;
  }

  nav .container{
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  nav .container h1{
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    font-size: 1.6rem;
  }

  ul{
    display: flex;
    list-style: none;
  }

  li{
    padding: 0 10px;
  }

  ul li a{
    text-decoration: none;
    color: #238068;
    transition: all 0.2s ease-in-out;
    position: relative;
    display: block;
  }

  ul li a::after{
    content: "";
    position: absolute;
    bottom: -2px;
    left: 0;
    width: 100%;
    height: 2px;
    background-color: #238068;
    transform-origin: left;
    transform: scaleX(0%);
    transition: transform 0.3s ease-in-out;
  }


  ul li a:hover{
    color: black;
  }

  ul li a:hover::after{
    transform: scaleX(100%);
  }

  @media (max-width: 514px){
    nav .container{
      flex-direction: column;
    }
    nav .container h1{
      text-align: center;
      margin-bottom: 10px;
    }
  }
</style>