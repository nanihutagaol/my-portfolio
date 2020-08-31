<template>
    <div class="x-experience x-flex-wrap">
        <div class="x-experience-img">
            <img :src="data.image" alt="image">
        </div>
        <div class="x-card">
            <h4>{{data.title}}</h4>
            <p> {{data.company}} </p>
            <p> <span> {{data.startDate}} - {{data.endData}} </span> <br>
                <span> {{data.location}} </span> <br>
                {{data.description}}
            </p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ExperienceCard',
    props: {
        data: {
            type: Object
        }
    },  
}
</script>

<style>
.x-experience img{
    border-radius: 6px;
    height: 65px;
}

.x-experience-img {
    padding: 0 1em 0 0;
}
</style>