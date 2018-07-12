<template>
  <div class="app">
    <div class="nav">
      <router-link to="/">Search</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <footer class=footer-box>
      <span class="copy-items">&copy; Copyright 2018 Sylwester Srokosz</span>
      <span class="copy-items">version: 0.0.1v</span>
    </footer>
    <router-view />
  </div>
</template>
<style lang="scss" scoped>
  body {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-size: 10px;
    font-family: Lato, sans-serif;
    color: #ffffff;
  }
  .nav {
    text-align: center;
    background-color: #52c3c0;
    border-bottom: 10px solid #311d5e;
    padding: 10px;
    border-bottom-right-radius: 25px;
    border-bottom-left-radius: 25px;


  }
  a{
    font-family: Lato, sans-serif;
    color: #fbff11;
    font-size: 1.4rem;
    text-decoration: none;
    display: inline;
    font-weight: 900;
  }
  .footer-box {
    font-size: 1rem;
    background-color: #52c3c0;
    border-radius: 10px;
    position: absolute;
    bottom: 0;
    right: 0;
  }
  .copy-items {
    display: inline-block;
    margin: 0.1rem;
  }
</style>

