<template>
    <div class="x-working">
        <p class="x-card-title">Experience</p>
        <div v-for="data in workingData" :key="data.title+data.company">
            <ExperienceCard :data="data"/>
        <hr>
        </div>
    </div>
</template>

<script>
import ExperienceCard from '@/components/Card/ExperienceCard.vue'

export default {
    name: 'Experience',
    components: {
        ExperienceCard
    },
    data() {
        return {
            workingData: [
                {
                    title: 'Software Development Engineer Intern',
                    image: 'https://media-exp1.licdn.com/dms/image/C4D0BAQHpXhPivbZyzA/company-logo_100_100/0?e=1606953600&v=beta&t=DUfNpN7rsR8fDCRDbKSPB1-Jhf7JDuVquZc9KtOtGsg',
                    company: 'GDP Labs',
                    startDate: 'Jun 2020',
                    endData: 'Aug 2020',
                    location: 'Jakarta, Indonesia',
                    description: 'Optimization of Docker Image Build Size and Time'
                },  
                {
                    title: 'Software Development Engineer Intern',
                    image: 'https://media-exp1.licdn.com/dms/image/C560BAQHTIx4znkcCEg/company-logo_100_100/0?e=1606953600&v=beta&t=arX6RA9HlIEuU_8m6OzGP0FL_-jlDRwBaNV7zU7dI_E',
                    company: 'Blibli.com',
                    startDate: 'Jun 2019',
                    endData: 'Sept 2019',
                    location: 'Jakarta, Indonesia',
                    description: 'Train UI Revamp'
                },
                {
                    title: 'Member of Blibli Future Program Batch 3.0',
                    image: 'https://media-exp1.licdn.com/dms/image/C560BAQHTIx4znkcCEg/company-logo_100_100/0?e=1606953600&v=beta&t=arX6RA9HlIEuU_8m6OzGP0FL_-jlDRwBaNV7zU7dI_E',
                    company: 'Blibli.com',
                    startDate: 'Aug 2018',
                    endData: 'Aug 2019',
                    location: 'Jakarta, Indonesia',
                    description: 'Joining bootcamp and working on project (1st and 2nd phase)'
                },  
                {
                    title: 'Leader of Departemen Agama dan Sosial BEM IT Del',
                    image: 'https://media-exp1.licdn.com/dms/image/C560BAQESCZFZZqVyng/company-logo_100_100/0?e=1606953600&v=beta&t=MBY8yNJeO8EzDqsVqLfWAa5z_j1tdVAMGdUEVvd6Kas',
                    company: 'Institut Teknologi Del',
                    startDate: 'May 2018',
                    endData: 'May 2019',
                    location: 'Sitoluama, Laguboti',
                    description: 'Coordinating the implementation of any spiritual activities'
                },  
            ]
        }
    }
}
</script>

<style>

</style>