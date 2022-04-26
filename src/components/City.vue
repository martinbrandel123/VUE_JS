<template>
    <div id="CityComponent">
      <div class="block">
        <h3>{{ name  }}</h3>
        <h3>{{ weather }}</h3>
        <h3>{{ temperature }}</h3>
        <h3>{{ updatedAt }}</h3>
      </div>
    </div>
</template>
  
<script>
export default {
  name: 'CityComponent',
  props:{
    'name' : String,
    'weather' : String,
    'temperature' : Number,
    'updatedAt' : String,
  },
}
</script>


<style scoped>

  .block{
    border: 1px black solid;
    width: 150px;
    margin: 15px auto;
  }

</style>
