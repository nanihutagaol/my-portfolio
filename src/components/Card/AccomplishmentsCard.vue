<template>
    <div class="x-card">
        <h4>{{data.title}}</h4>
        <p> {{data.endDate ? data.startDate + ' - ' + data.endDate : data.startDate}} | {{data.provider}} </p>
        <img v-if="data.image" :src="data.image" alt="image">
        <p class="x-card-description" v-html="data.description"></p>
    </div>
</template>

<script>
export default {
    name: 'AccomplishmentsCard',
    props: {
        data: {
            type: Object
        }
    },  
}
</script>

<style>
img {
    width: 100%;
}

.x-card-description {
    margin-top: 1em;
}

.x-card-description ul li{
    font-size: 14px;
    width: 100%;
    line-height: 18px;
}
</style>