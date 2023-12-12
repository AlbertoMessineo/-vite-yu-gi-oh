<script>
    import CardsCollection from './CardsCollection.vue';

      export default{
        name: 'AppMain',
        components: {
            CardsCollection,
        }
    };
</script>

<template>
    
        
   
    <!-- contenitore carte -->
    <div class="container main p-4">
        <div class="col-2 mb-4 pt-3">
            <select id="inputState" class="form-select">
                <option selected>Alien</option>
                <option>...</option>
            </select>
        </div>
        <div class="container found p-4">
            <h3>Found 39 cards</h3>
        </div>
       <CardsCollection class="collection"/> 
    </div>
    
</template>

<style scoped>


</style>
