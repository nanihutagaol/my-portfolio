<template>
    <div class="x-honors-awards">
        <p class="x-card-title">Honors and Awards</p>
        <div v-for="data in honorsData" :key="data.title+data.provider">
            <AccomplishmentsCard :data="data"/>
        <hr>
        </div>
    </div>
</template>

<script>
import AccomplishmentsCard from '@/components/Card/AccomplishmentsCard.vue'

export default {
    name: 'HonorsAwards',
    components: {
        AccomplishmentsCard
    },
    data() {
        return {
            honorsData: [
                {
                    title: 'Candidate Test of Mahasiswa Berprestasi Tingkat Nasional 2019 - Diploma',
                    image: require('@/assets/pilmapres.jpg'),
                    startDate: 'Apr 2019',
                    provider: 'Institut Teknologi Del',
                    description: 'The annual program of Kemenristekdikti in order to appreciates students, who are able to balance their lectures, organizations, and extracurricular activities <br> <a href="https://www.youtube.com/watch?v=CZSC6QJQWqc&t=12s"> Visit Youtube to see my selection video.</a>'
                },  
                {
                    title: 'Role Model Student 2018',
                    image: require('@/assets/best-student-award.jpg'),
                    startDate: 'Sept 2018',
                    provider: 'Institut Teknologi Del',
                    description: 'Role model student award is a campus award given to one student in the 3rd year, who has good performance in academic and non academic section, and also can be role model to other students'
                },  
                {
                    title: 'Finalist of Bukalapak Programming Contest Season 4 Regional Sumatera',
                    image: require('@/assets/blpc.png'),
                    startDate: 'Nov 2016',
                    provider: 'Bukalapak',
                    description: ''
                }
            ]
        }
    }
}
</script>

<style>

</style>