<template>
  <div class="x-home">
    <MainBanner :name="name"/>
    
    <div class="x-flex-wrap col-md-12">
        <div class="col-md-1"></div>
        <div class="x-card-shadow col-md-3">
          <ProfileInformation/>
        </div>
        <div class="x-content-data col-md-7">
            <div id="experience">
              <Experience class="x-card-shadow"/>
            </div>
            <div id="projects">
              <Projects class="x-card-shadow"/>
            </div>
            <div id="honors">
              <HonorsAwards class="x-card-shadow"/>
            </div>
            <div id="organizations">
              <Organizations class="x-card-shadow"/>
            </div>
        </div>
    </div>
    
    <Footer :isPanelActive="isPanelActive"/>
  </div>
</template>

<script>
import MainBanner from '@/components/AboutMe/MainBanner.vue'
import ProfileInformation from '@/components/AboutMe/ProfileInformation.vue'
import Experience from '@/components/AboutMe/Experience.vue'
import HonorsAwards from '@/components/AboutMe/HonorsAwards.vue'
import Organizations from '@/components/AboutMe/Organizations.vue'
import Projects from '@/components/AboutMe/Projects.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'Home',
  components: {
    MainBanner,
    ProfileInformation,
    Experience,
    HonorsAwards,
    Organizations,
    Projects,
    Footer
  },
  data() {
    return {
      isPanelActive: true,
      name: 'Nani Renova Hutagaol',
      highlightsContent: [
        {
          title: 'Consult',
          description: 'Co-create, design thinking; strengthen infrastructure resist granular. Revolution circular, movements or framework social impact low-hanging fruit. Save the world compelling revolutionary progress.',
          icon: 'fa fa-comments-o'
        },
        {
          title: 'Design',
          description: 'Policymaker collaborates collective impact humanitarian shared value vocabulary inspire issue outcomes agile. Overcome injustice deep dive agile issue outcomes vibrant boots on the ground sustainable.',
          icon: 'fa fa-paint-brush'
        },
        {
          title: 'Develop',
          description: 'Revolutionary circular, movements a or impact framework social impact low-hanging. Save the compelling revolutionary inspire progress. Collective impacts and challenges for opportunities of thought provoking.',
          icon: 'fa fa-cubes'
        },
        {
          title: 'Marketing',
          description: 'Peaceful; vibrant paradigm, collaborative cities. Shared vocabulary agile, replicable, effective altruism youth. Mobilize commitment to overcome injustice resilient, uplift social transparent effective.',
          icon: 'fa fa-bullhorn'
        },
        {
          title: 'Manage',
          description: 'Change-makers innovation or shared unit of analysis. Overcome injustice outcomes strategize vibrant boots on the ground sustainable. Optimism, effective altruism invest optimism corporate social.',
          icon: 'fa fa-tasks'
        },
        {
          title: 'Evolve',
          description: 'Activate catalyze and impact contextualize humanitarian. Unit of analysis overcome injustice storytelling altruism. Thought leadership mass incarceration. Outcomes big data, fairness, social game-changer.',
          icon: 'fa fa-line-chart'
        }
      ]
    }
  }
}

</script>

<style>
.x-home {
    position: absolute;
    z-index: 0;
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}

.x-content-data {
  margin-right: -10px;
  margin-left: 10px;
  text-align: justify;
}

/* Global CSS */
.x-flex-wrap {
  display: flex;
  flex-wrap: wrap;
}

.x-card-title {
  margin: 0 0 0.75em 0;
  font-size: 26px;
  color: #3594dd;
}

.x-card-shadow {
   box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
   border-radius: 5px;
   padding: 20px;
   margin-top: 20px;
}

.x-card h4 {
    font-size: 18px;
    line-height: 16px;
}

.x-card p {
    font-size: 15px;
    line-height: 18px;
    /* font-family: Arial, Helvetica, sans-serif; */
}

.x-card p span {
    font-size: 14px;
    color: rgba(34, 34, 34, 0.6);
}
</style>