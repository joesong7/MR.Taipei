<template>
<div class="card w-100">
  <div class="card-body">
    <div class="container">
  <div class="row">
    <div class="col">
      起點
      <br>
      <v-text>租屋處</v-text>
    </div>
    <div class="col">
      目的地
      <br>
       <v-text>實踐大學</v-text>
    </div>
    
  </div>
</div>
     <div class="progress" >

  <div class="progress-bar" role="progressbar" style="width: 50%" aria-valuenow="15" aria-valuemin="0" aria-valuemax="100"></div>
  <div class="progress-bar bg-success" role="progressbar" style="width: 50%" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100"></div>


  

</div>
<div class="container">
  <div class="row">
    <div class="col">
      Column
    </div>
    <div class="col">
      Column
    </div>
  </div>
</div>
  </div>
</div>

</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
 setup() {
  
  

  


}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
