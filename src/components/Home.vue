<template>
    <div>
        <h1>Liste des séries</h1> 
        <ul>
            <serie v-for="serie in series" :serie="serie" @selectionneSerie="ajouteSupprimeSerie"></serie>
        </ul>
    </div>
</template>

<script>
import Serie from '@/components/Serie.vue'
import seriesService from '@/services/series.service'

export default {
    components: {
        Serie
    },
    data(){
        return {series: []}
    },
    mounted () {
        seriesService.getSeries().then(response => this.series = response.map(item => item.show))
    }, methods:{
        ajouteSupprimeSerie() {
            appel du service;
        }
    }
}
</script>

<style scoped>
	ul {
		padding: 50px;
	}
</style>
