<template>
  <div class="wrapper">
    <div class="asset-box">
      <img src="../assets/Pokeball.png" alt="" srcset="">
    </div>
    <article class="about">
      <h1>PokeData</h1>
      <h3>This a small Pokémon Encyclopedia written in Vue.js, using external APIs.</h3>
      <p>try it, test it, enjoy it!</p>
    </article>
  </div>
</template>

<script>
export default {
  name: 'About',
  components: {},
};
</script>

<style>
  body {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-size: 10px;
  }
  .wrapper {
  background-size: no-repeat;
  background-image: linear-gradient(to right, #09052f 0%, #311d5e 100%);
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  margin: 0;
  padding: 0;
  height: 91.6vh;
  font-family: Lato, sans-serif;
  color: #ffffff;
  }
  h1 {
    color: #fbff11;
    margin: 2rem;
    font-size: 4rem;
    letter-spacing: 6px;
  }
  h3 {
    margin: 0;
    font-size: 1.5rem;
  }
  p {
    margin: 0.5rem;
    font-size: 1.2rem;
  }
  .img {
    border: 10px solid #ffffff;
  }

</style>

