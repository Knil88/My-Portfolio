<script>
export default{
  data() {
    return {
      contacts:[{'image':'linkedin.png',
                  'text':'Il mio profilo Linkedin',
                  'link':'https://www.linkedin.com/in/yarinarducci/',
                  },
                  {'image':'github.svg',
                  'text':'Il mio profilo Github',
                  'link':'https://github.com/Knil88',
                  },
                  {'image':'gmail.svg',
                  'text':'narducciyari@gmail.com',
                  'link':'#',
                  },
                
                ]
    }
  },
}
</script>

<template>

    <h2 class="text-center text-white my-3" id="MyContacts">My contacts</h2>
    <div class="w-75 m-auto ">
        <div style="width: 100%"><iframe scrolling="no" marginheight="0" marginwidth="0" src="https://maps.google.com/maps?width=100%25&amp;height=500&amp;hl=en&amp;q=Via%20dell'olmata%2090%20+(My%20Business%20Name)&amp;t=&amp;z=14&amp;ie=UTF8&amp;iwloc=B&amp;output=embed" width="100%" height="500" frameborder="0"><a href="https://www.maps.ie/distance-area-calculator.html">measure acres/hectares on map</a></iframe></div>
    </div>
   <footer >
        <div  id="link_container" v-for="contact in contacts">
           <div class="link-contact mx-3 my-2">
            <img :src="contact.image" alt="">
             <a  class="text-white text-decoration-none mx-3" :href="contact.link">{{contact.text}}</a>
           </div>
         
        </div>
   </footer>
        
    
</template>

<style lang="scss">

footer{
    border: 1px solid white;
    background-color: rgba($color: #000000, $alpha: 0.5);
    backdrop-filter: blur(4px);
    margin: 0 auto;
    width: 100vw;
    overflow: hidden;
    
  
    padding: 20px;
  }
  .link_contact{
  
   margin-bottom: 5px;
  }
  .link-contact img{
    width: 50px;
  
    
    margin-left: 10px;
  }
  #link_container{
    display: flex;
    justify-content: space-around;
    flex-direction: column;
  }
 
  
  
</style>