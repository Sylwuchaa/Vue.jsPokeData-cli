<template>
  <div class="wrapper">
    <div class="asset-box">
      <img src="./../assets/Pokedex.png" alt="pokedex" srcset="">
    </div>
    <div class="search">
    <label for="search">Search</label>
    <input id="search"
    name="search"
    v-model="searchValue" 
    @input="handleInput"
    />
    </div>
  </div>
</template>
<script>
import axios from 'axios';

const API = 'http://pokeapi.co/media/sprites/pokemon/';
export default {
  name: 'Search',
  data() {
    return {
      searchValue: '',
    };
  },
  methods: {
    handleInput() {
      axios.get(`${API}${this.searchValue}.png`)
      .then((response) => {
        console.log(response);
      })
      .catch((error) => { 
        console.log(error);
      });
    },
  },
};
</script>

<style lang="scss" scoped>
  body {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-size: 10px;
    font-family: Lato, sans-serif;
    color: #ffffff;
    position: relative;
    width: 100%;
    height: 100%; 
  }
  html {
    font-size: 10px;
    position: unset;
    width: 100%;
    height: 100%; 
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
    // height: 91.6vh;
  }
  .search {
    text-align: center;
    color: #13102d;
    width: 35rem;
    display: flex;
    flex-direction: column;
    width: 18rem;

  label {
    padding-bottom: 1.5rem;
    font-size: 3.0rem;
    font-weight: 300;
    color: #ffffff;
  }
  input {
    padding: 0.3rem;
    font-family: Lato, sans-serif;
    border-radius: 3rem;
    height: 2.5rem;
    border: 0;
    border-bottom: 4px solid #52c3c0;
    font-size: 2rem;
    color: black;

  }
}
</style>
