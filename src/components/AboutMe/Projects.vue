<template>
    <div class="x-projects">
        <p class="x-card-title">Projects</p>
        <div v-for="data in organizationsData" :key="data.title+data.provider">
            <AccomplishmentsCard :data="data"/>
        <hr>
        </div>
    </div>
</template>

<script>
import AccomplishmentsCard from '@/components/Card/AccomplishmentsCard.vue'

export default {
    name: 'Projects',
    components: {
        AccomplishmentsCard
    },
    data() {
        return {
            organizationsData: [
                {
                    title: 'Blibli Bazaar',
                    startDate: 'Feb 2019',
                    endDate: 'Aug 2019',
                    provider: 'Blibli Future Program',
                    description: 
                        '<ul>' + 
                            '<li>Blibli Future Program project. This system used to handle the current office bazaar.</li>' + 
                            '<li>FE: https://github.com/reboot16/otob_fe</li>' + 
                            '<li>BE: https://github.com/alexandernsalim/otob</li>' + 
                            '<li>Used: VueJS, Bootstrap, Java SpringBoot, MongoDB</li>' + 
                        '</ul>'
                },  
                {
                    title: 'Sistem Penganggaran Dana',
                    startDate: 'Feb 2019',
                    endDate: 'May 2019',
                    provider: 'Institut Teknologi Del',
                    description: 
                        '<ul>' + 
                            '<li>Module development of Campus Information System (CIS)</li>' + 
                            '<li>Used: Yii2, MySQL</li>' + 
                        '</ul>'
                },
                {
                    title: 'Inventory Management System',
                    startDate: 'Aug 2018',
                    endDate: 'Jan 2019',
                    provider: 'Blibli Future Program',
                    description: 
                        '<ul>' + 
                            '<li>Blibli Future Program project. This system used to manage inventory data when user want to borrow an item.</li>' + 
                            '<li>Used: HTML, CSS, JS, Bootstrap, Java SpringBoot, MongoDB</li>' + 
                        '</ul>'
                },
                {
                    title: 'Surat Cuti Izin Pegawai',
                    startDate: 'Feb 2018',
                    endDate: 'May 2018',
                    provider: 'Institut Teknologi Del',
                    description: 
                        '<ul>' + 
                            '<li>Module development of Campus Information System (CIS)</li>' + 
                            '<li>Used: Yii2, MySQL</li>' + 
                        '</ul>'
                },
                {
                    title: 'Aplikasi Promosi dan Pemesanan UKM Banana Boat',
                    startDate: 'Jan 2017',
                    endDate: 'Jun 2017',
                    provider: 'Institut Teknologi Del',
                    description: 
                        '<ul>' + 
                            '<li>Website that used to get an information about Lumban Bulbul and also can book the facility, like Banana Boat.</li>' + 
                            '<li>Used: PHP, MySQL, HTML, CSS, JS, Bootstrap</li>' + 
                        '</ul>'
                },
            ]
        }
    }
}
</script>

<style>

</style>