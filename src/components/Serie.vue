<template>
    <li class="list-group-item" @click="onClick()">
        <div class="media">
            <div class="media-left" v-if="serie.image">
                <img class="media-object" :src="serie.image.medium" />
            </div>
            <div class="media-body">
                <h4 class="media-heading">{{ serie.name }}</h4>
                <div v-html="serie.summary"></div>
            </div>
        </div>
    </li>
</template>

<script>
export default {
    props: [
        'serie'
    ],
    methods: {
        onClick(){
            console.log(this.serie)
            this.$emit('selectionneSerie', this.serie)
        }
    }
}
</script>

<style>
.list-group-item {
    position: relative
}

.media {
    text-align: left;
}

.media-object {
    height: 64px;
}
</style>
