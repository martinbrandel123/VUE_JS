<template>
  <div class="home">
    <CityComponent/>
  </div>
</template>

<script>
// @ is an alias to /src
import CityComponent from '@/components/CitiesList.vue'

export default {
  name: 'HomeView',
  components: {
    CityComponent
  }
}
</script>