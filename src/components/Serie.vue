<template>
    <div>
        <h1>Série</h1> 
        <div>{{name}}</div>
        <div>{{summary}}</div>
       <img v-bind:src="image.medium" />
    </div>
</template>

<script>
export default {
    data() {
        return {
            name: 'NightClazz',
            summary: 'Wha an amazing codelab...',
            image: {medium:'static/logo.png'}
        }
    }
}
</script>
    

<style>

</style>
