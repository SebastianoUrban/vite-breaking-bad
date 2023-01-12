<template>
  <div>
    <div>
      <h3>Numero di carte: {{ cards.length }}</h3>
    </div>
    <div  class=" d-flex justify-content-between flex-wrap">
      <SingleCard v-for="card in cards" 
      :name = "card.name"
      :archetype = "card.archetype"
      :image = "card.card_images[0].image_url"/>
    </div>
  </div>
</template>

<script>
  import axios from 'axios';
  import SingleCard from './SinglCard.vue';

  export default {
    data() {
      return {
        cards : []
      }
    },
    methods: {
      getCards () {
        axios.get('https://db.ygoprodeck.com/api/v7/cardinfo.php', {
          params : {
            num : 10,
            offset : 0
          }
        })
        .then( (response) => {
          this.cards = response.data.data;
        })
        .catch( function (error){
          console.log(error);
        })
      }
    },
    created () {
      this.getCards();
    },
    components : {
      SingleCard
    }
  }
</script>

<style lang="scss" >

  
</style>