<script>
import Header from './components/Header.vue';
import SectionAbout from './components/SectionAbout.vue';
import SectionSkills from './components/SectionSkills.vue'
import SectionProject from './components/SectionProject.vue';
import Footer from './components/Footer.vue';




export default{

  data() {
  return {
    isLoaded:false,
  }
},
mounted() {
    //metodo che crea un pagina di caricamento
    setTimeout(() => {
      this.isLoaded = true
    }, 4000);
  },
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
  
 

 <div class="text-center" v-if="!isLoaded">
    
  <div class="Flex_Load">
   <div class="pos_img">
     <img class="img_loading" src="./assets/AP_LWHITE.png" alt="">
   </div>
   <img id="loader"  src="./assets/Eclipse-1s-200px.svg" alt="">
  </div>
 </div >
<div v-else>
  <Header/>
 <main>
  <SectionAbout/>
  <SectionSkills/>
  <SectionProject/>
 </main>
 <Footer/>
</div>

</template>

<style >
.lds-facebook {
  display: inline-block;
  position: relative;
  width: 80px;
  height: 80px;
}
.lds-facebook div {
  display: inline-block;
  position: absolute;
  left: 8px;
  width: 16px;
  background: #fff;
  animation: lds-facebook 1.2s cubic-bezier(0, 0.5, 0.5, 1) infinite;
}
.lds-facebook div:nth-child(1) {
  left: 8px;
  animation-delay: -0.24s;
}
.lds-facebook div:nth-child(2) {
  left: 32px;
  animation-delay: -0.12s;
}
.lds-facebook div:nth-child(3) {
  left: 56px;
  animation-delay: 0;
}
@keyframes lds-facebook {
  0% {
    top: 8px;
    height: 64px;
  }
  50%, 100% {
    top: 24px;
    height: 32px;
  }
}
</style>
