<template>
<div class="card">
<div class="card-img">
    <img class="team-img" src="http://2.bp.blogspot.com/-L_vBOvPOMtk/TsrU1EOBpWI/AAAAAAAAAfQ/uHIa7_9oGdM/s1600/Thomas%2BNumme.jpg"alt="Card image cap"/>
</div>
<div class="card-content">
    <div class="teamName"><h1>Lagnavn</h1></div>
    <div class="teamMembers"><h3>'Filip og Carl'</h3></div>
</div>
</div>
</template>

<script>
export default {
  name: 'Card',
  data () {
    return {
      msg: 'This is a card'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .card{
    height: 50%;
    width: 50%;
    margin: 0;
    padding: 0; 
    border: 5px solid red  ;
  }
  .team-img{
    max-width: 100%;
    height: auto;
  }

  h1,h3{
    align-content: center;
    color: red;
  }

</style>
