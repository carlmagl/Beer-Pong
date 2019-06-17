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
          { id: 1, title: 'Lag 1'},
          { id: 2, title: 'Lag 2'},
          { id: 3, title: 'Lag 3'},
          { id: 4, title: 'Lag 4'}
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