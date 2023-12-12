<script>
      export default{
        name: 'Card',
        props: ['name' , 'archetipo' , 'img'],
    };
</script>

<template>
  <div class="yugi-card">
    <div>
      <img :src="img" :alt="name">
    </div>
    <h4> {{ name }}</h4>
    <h6 class="align-self-end">{{ archetipo }}</h6>
  </div>
</template>

<style scoped>


</style>
