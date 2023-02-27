<script>
import Header from './components/Header.vue';
import SectionAbout from './components/SectionAbout.vue';
import SectionSkills from './components/SectionSkills.vue'
import SectionProject from './components/SectionProject.vue';
import Footer from './components/Footer.vue';


export default{
  components:{
    Header,
    SectionAbout,
    SectionSkills,
    SectionProject,
    Footer,


    
    
  }
}

</script>

<template>
 <Header/>
 <main>
  <SectionAbout/>
  <SectionSkills/>
  <SectionProject/>
 </main>
 <Footer/>
</template>

<style >

</style>
