<template>
  <div class="hello">
    <CityComponent :name="name" :weather="weather" :temperature="temperature" :updatedAt="updatedAt">
      
    </CityComponent>
  </div>
</template>

<script>

import CityComponent from './City.vue'
import { format } from '/node_modules/timeago.js';

export default {
  components: { CityComponent },
   name : 'HelloWorld',
   data(){
        return {
            name: 'Ma ville', 
            weather: 'Peu nuageux', 
            temperature: 20.55, 
            updatedAt: format(new Date())
        }
    },
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
