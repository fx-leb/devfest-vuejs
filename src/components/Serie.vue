<template>
    <div>
        <h1>{{name}}</h1> 
        </div>{{summary}}</div>
        <img v-bind="image.medium"/>
    </div>
</template>

<script>
export default {
    data() {
        return 
        {
            name: 'NightClazz',
            summary: 'Wha an amazing codelab...',
            image: {medium:'static/logo.png'}
        };
    }
}
</script>
    

<style>

</style>
