<template>
    <div class="x-organizations">
        <p class="x-card-title">Organizations</p>
        <div v-for="data in organizationsData" :key="data.title+data.provider">
            <AccomplishmentsCard :data="data"/>
        <hr>
        </div>
    </div>
</template>

<script>
import AccomplishmentsCard from '@/components/Card/AccomplishmentsCard.vue'

export default {
    name: 'Organizations',
    components: {
        AccomplishmentsCard
    },
    data() {
        return {
            organizationsData: [
                {
                    title: 'Departemen Agama dan Sosial',
                    image: require('@/assets/depagsos.jpg'),
                    startDate: 'May 2017',
                    endDate: 'May 2019',
                    provider: 'Institut Teknologi Del',
                    position: 'Member (1st year), Leader (2nd year)',
                    description: 'Departement Agama dan Sosial is a students organization that standing under BEM IT Del. This Department aims to facilitate students in developing themselves actively in the field of spirituality and social.'
                },  
                {
                    title: 'Himpunan Mahasiswa Diploma Empat Teknik Informatika',
                    image: '',
                    startDate: 'Sept 2016',
                    endDate: 'Sept 2020',
                    provider: 'Institut Teknologi Del',
                    position: 'Anggota',
                    description: 'Organizations to establish student character and self-reliance'
                }
            ]
        }
    }
}
</script>

<style>

</style>