<template>
  <div id="app">
    <app-header></app-header>
    <app-window></app-window>

  </div>
</template>

<script>
import Header from './components/Header'
import Window from './components/Window'

export default {
  name: 'app',
  data(){
    return{
      bill: 0,
      ratings: 0,
      people:0,
      selectpeople:0
    }
  },
  components: {
    appHeader: Header,
    appWindow: Window
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  border: 2px solid #000;
  color: #2c3e50;
  margin: 60px auto auto auto;
  width: 800px;
  height: 100%;
  padding: 3%;
}
</style>
