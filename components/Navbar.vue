<template>
  <nav>
    <div class="container">
      <h1>Hacktoberfest Satrter Repo</h1>
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
  }

  ul li a:hover{
    color: black;
  }
</style>