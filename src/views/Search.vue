<template>
  <div class="wrapper">
    <div class="search">
    <label for="search">Search</label>
    <input id="search" name="search" />
    </div>
  </div>
</template>
<script>
export default {
  name: 'Search',
  components: {},
};
</script>

<style lang="scss" scoped>
.wrapper {
  background-size: no-repeat;
  background-image: linear-gradient(to right, #09052f 0%, #311d5e 100%);
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  margin: 0;
  padding: 0;
  height: 90vh;
}
.search {
  text-align: center;
  color: #13102d;
  width: 350px;
  display: flex;
  flex-direction: column;
  width: 250px;

  label {
    padding-bottom: 15px;
    font-family: Lato, sans-serif;
    font-size: 35px;
    color: #ffffff;
    font-weight: 300;
  }
  input {
    padding: 3px;
    font-family: Lato, sans-serif;
    border-radius: 30px;
    height: 30px;
    border: 0;
    border-bottom: 4px solid #52c3c0;
    font-size: 20px;
    color: black;

  }
}
</style>
