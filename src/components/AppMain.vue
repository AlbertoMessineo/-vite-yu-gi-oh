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
    <div class="container">
       <CardsCollection /> 
    </div>
    
</template>

<style scoped>


</style>
