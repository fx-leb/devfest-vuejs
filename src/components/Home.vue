<template>
    <div>
        <h1>Liste des séries</h1> 
        <ul>
            <serie></serie>
            <serie></serie>
            <serie></serie>
            <serie></serie>
        </ul>
    </div>
</template>

<script>

import Serie from '@/components/Serie.vue'
import api from '@/services/series.service.js'

export default {
    components: {
        Serie,
        },
      mounted() {
          api.getSeries().then(series => console.log(series.map(serie => serie.show)))
      }  
        
}
</script>

<style scoped>
	ul {
		padding: 50px;
	}
</style>
