<template>
  <v-app>
    <v-main >
      
      <div id="pageContainer">
        <div id="header">
          
          <PageHeader/>
          
        </div>
          <div id="contentContainer">
            <div id="skills">
              <TechnicalSkills/>
            </div>
        
            <div id="aboutMe">
              <AboutMe/>
            </div>
        
            <div id="projects">
              
              <MyProjects/>
              
            </div>
        
            <div id="contact">
              <ContactMe/>
            </div>
          </div>
        <div id="footer">
          <PageFooter/>
        </div>
      </div>
    </v-main>
  </v-app>
</template>

<script>
import PageHeader from '@/components/PageHeader.vue'
import TechnicalSkills from '@/components/TechnicalSkills.vue'
import AboutMe from '@/components/AboutMe.vue'
import MyProjects from '@/components/MyProjects.vue'
import ContactMe from '@/components/ContactMe.vue'
import PageFooter from '@/components/PageFooter.vue'


export default {
  name: 'App',
  components: {
    PageHeader,
    TechnicalSkills,
    AboutMe,
    MyProjects,
    ContactMe, 
    PageFooter
    
  },

  data: () => ({
    //
  }),
};
</script>

<style lang="scss" scoped>
#pageContainer{
  display: grid;
  grid-template-rows: 0.5fr 5fr 0.5fr;
  
  background-color: rgb(97, 106, 114);

  #header{
    position: relative;
    display: grid;
    grid-row: 1;
    
  }
  #footer{
    position: relative;
    display: grid;
    grid-row: 6;
  }
  #contentContainer{
    display: grid;
    grid-template-rows: 1fr 1fr 1fr 1fr;
    #skills{
    position: relative;
    display: grid;
    grid-row: 1;
  }
  #aboutMe{
    position: relative;
    display: grid;
    grid-row: 2;
  }
  #projects{
    position: relative;
    display: grid;
    grid-row: 3;
  }
  #contact{
    position: relative;
    display: grid;
    grid-row: 4;
  }
  }
  
  
}

</style>
