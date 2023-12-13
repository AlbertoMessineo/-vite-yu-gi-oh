<script>
      export default{
        name: 'Card',
        props: ['name' , 'archetipo' , 'img'],
    };
</script>

<template>
  <div class="yugi-card m-2">
    <div>
      <img class="card-img" :src="img" :alt="name">
    </div>
    <h4 class="text-center m-2"> {{ name }}</h4>
    <h6 class="align-self-end text-center m-2">{{ archetipo }}</h6>
  </div>
</template>

<style scoped>


</style>
