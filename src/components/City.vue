<template>
    <div id="CityComponent">
        <h3>{{ name  }}</h3>
        <h3>{{ weather }}</h3>
        <h3>{{ temperature }}</h3>
        <h3>{{ updatedAt }}</h3>

        <!-- <h2>{{ weather  }}</h2>
        <h3>{{ temperature  }}</h3>
        <h3>{{  updatedAt.toLocaleString()   }}</h3> -->
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

</style>
