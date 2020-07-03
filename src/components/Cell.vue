// This is the individual cell componet

<template>
    <td class="cell" @click="test">{{ mark }}</td>
</template>

<script>

export default {
  data(){
    return{
      mark:"",
      currentPlayer:"X"
    }
  },
  methods:{
    //method to create X and O on the cell
    test:function () {
        //console.log(this.currentPlayer)
        this.mark=this.currentPlayer;
        this.currentPlayer=this.currentPlayer==="X" ? this.currentPlayer="O":this.currentPlayer="X";
        //console.log(this.currentPlayer)
    }
  }
}
</script>

<style>

.cell {
  width: 33.333%;
  height: 90px;
  border: 6px solid #2c3e50;
  font-size: 3.5em;
  font-family: 'Avenir', Helvetica, sans-serif;
}

</style>