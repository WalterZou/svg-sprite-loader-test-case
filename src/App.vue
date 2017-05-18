<template>
  <div id="app">
    <img src="./assets/logo.svg">
    <hello></hello>
    <div class="logo"></div>
  </div>
</template>

<script>
  import Hello from './components/Hello'
  import Logo from './assets/logo.svg'
  console.log(Logo)
  export default {
    name: 'app',
    components: {
      Hello
    },
    mounted() {
      console.log(Logo)
    }
  }

</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
  img{
    width: 100px;
    height: 100px;
    background: #eee;
  }
  .logo {
    width: 200px;
    height: 200px;
    margin: 0 auto;
    background-image: url('./assets/logo.svg');
    background-color: #eee;
  }

</style>
