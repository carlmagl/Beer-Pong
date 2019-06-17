<template>
  <div class="root">
    <ul id="list">
      <li v-for="card in cards">
        <Card v-bind:card="card"/>
      </li>
    </ul>

    <div @click="add" class="add-button">Trykk her</div>
    <input type ="number" @click="reset(number)" class="reset">Reset</div>

  </div>
</template>

<script>
  import Card from './Card'
  export default { 
    components:{
      Card
    },
    data() {
      return {
        cards: [
          { id: 1, title: 'Lag 1', members: "Carl og Filip", url:['https://dbstatic.no/66617101.jpg?imageId=66617101&x=0&y=0&cropw=100&croph=99.9&width=640&height=494']},
          { id: 2, title: 'Lag 2', members: "Ander og Sigg", url:['https://dbstatic.no/66617093.jpg?imageId=66617093&x=0&y=0&cropw=100&croph=100&width=640&height=412']},
          { id: 3, title: 'Lag 3', members: "Ulrik og Jacob", url:['https://dbstatic.no/66617095.jpg?imageId=66617095&x=0&y=0&cropw=100&croph=99.9&width=640&height=496']},
          { id: 4, title: 'Lag 4', members: "Nissen og Rudolf", url:['https://dbstatic.no/66617091.jpg?imageId=66617091&x=0&y=0&cropw=100&croph=100&width=640&height=394']}
        ],
      }
    },
    methods: {
      add() {
        this.cards.push({ id: 4, title: 'Lag 4'});
      },
      reset(id) {
        this.cards = this.cards.filter(todo => todo.id !== id);
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h1,
  h2 {
    font-weight: normal;
  }

  ul {
    list-style-type: none;
    padding: 0;
    margin: 0 auto;
  }

  li {
    display: inline-block;
    margin: 0 10px;
    vertical-align: top;
  }

  a {
    color: #42b983;
  }

  .test {
    font: 20;
    position: relative;
  }
</style>