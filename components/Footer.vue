<template>
  <footer>
    <div class="container">
      For Hacktoberfest 2020 - Beginners' repo
    </div>
  </footer>
</template>

<style scoped>
  footer {
    padding: 20px 0;
    background-color: #eee;
  }

  footer .container{
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