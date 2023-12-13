<script>
    import CardsCollection from './CardsCollection.vue';

      export default{
        name: 'AppMain',
        components: {
            CardsCollection,
        },
        data(){
            return{
                selectKey: '',
            };
        },
    };
</script>

<template>
    
        
   
    <!-- contenitore carte -->
    <div class="container main p-4">
        <div class="col-2 mb-4 pt-3">
            <select id="inputState" class="form-select" v-model="selectKey">
                <option selected value="Seleziona Archetipo">Seleziona archetipo</option>
                <option value="Alien">Alien</option>
                <option value="Infernoble Arms">Infernoble Arms</option>
                <option value="Noble Knight">Noble Knight</option>
                <option value="Melodious">Melodious</option>
                <option value="Archfiend">Archfiend</option>
                <option value="Umi">Umi</option>
                <option value="Elemental HERO">Elemental HERO</option>
                <option value="ABC">ABC</option>
                <option value="A.I.">A.I.</option>
                <option value="@Ignister">@Ignister</option>
            </select>
        </div>
        <div class="container found p-4">
            <h3>Found 40 cards</h3>
        </div>
       <CardsCollection class="collection"/> 
    </div>
    
</template>

<style scoped>


</style>
