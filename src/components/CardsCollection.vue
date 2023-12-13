<script>
import axios from 'axios';
    import Card from './Card.vue';
      export default{
        name: 'CardsCollection',
        components:{
            Card,
        },
        data(){
            return{
                cards:[],
                APIurl:'https://db.ygoprodeck.com/api/v7/cardinfo.php?num=20&offset=0',
            };
        },
        created(){
            axios.get(this.APIurl).then((response) => {
                this.cards = response.data.data;
            });
        }
    };
</script>

<template>
    <!-- <div class="container found">
        Found 39 cards
    </div> -->
    <div class="d-flex flex-wrap justify-content-around gap-3 p-5">
        <Card v-for="card in cards" 
        :name="card.name"
        :archetipo="card.archetype"
        :img="card.card_images[0].image_url"/>
    </div>
     
</template>

<style scoped>


</style>
