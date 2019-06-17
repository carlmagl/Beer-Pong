<template>
  <div class="root">
    <div class="test">a</div>
    <div class="test">s</div>
    <div class="test">s</div>
    <div class="test">s</div>
    <div class="test">s</div>
  </div>
</template>

<script>
export default {
  name: 'cardList',
  data () {
    return {
      msg: 'Hei'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
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

.test{
  font: 20;
  position: relative;
}

</style>
