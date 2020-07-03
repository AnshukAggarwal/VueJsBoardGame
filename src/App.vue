// This is the main component which renders the grid on the page
<template>
  <div>
    <div id="app">
      <div id="details">
        <h1>Tic Tac Toe</h1>
      </div>
      <h3>Match Number : {{matches}}</h3>
      <h3>It is {{player}}'s turn</h3>
      <Grid :currentPlayer="player"/>
      <button @click="restart">Restart</button>
    </div>
  </div>
</template>

<script>
import Grid from './components/Grid.vue'
export default {
  components:{Grid},
  name: 'App',
  data(){
    return{
      player:"X",
      matches:0
    }
  },
  methods:{
    //method to increment the game number
    restart:function (){
      this.matches++;
    }
  }
}
</script>

<style>

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
h1 {
  text-transform: uppercase;
  font-weight: bold;
  font-size: 3em;
}

</style>
