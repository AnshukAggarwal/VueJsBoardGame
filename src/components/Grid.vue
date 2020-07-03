/* //this component takes care of the board/grid.
// it requires the grid component
//here we need a 3x3 grid, hence 3 trs */
<template>
  <div>
    <table class="grid">
      <tr>
        <cell name="1"></cell>
        <cell name="2"></cell>
        <cell name="3"></cell>
      </tr>
      <tr>
        <cell name="4"></cell>
        <cell name="5"></cell>
        <cell name="6"></cell>
      </tr>
      <tr>
        <cell name="7"></cell>
        <cell name="8"></cell>
        <cell name="9"></cell>
      </tr>
    </table>
  </div>
</template>
<script>
import Cell from './Cell.vue'
export default {
  name:"Grid",
  components:{Cell},
  data(){
    return{

    }
  }
}
</script>

<style>
.grid {
  background-color: #34495e;
  color: #fff;
  width: 50%;
  border-collapse: collapse;
  margin: 0 auto;
}

</style>
