<script>

export default{
    data() {
        return {
           
            
            links:[
                {'name':'Home',
                 'anchor':'#Home',
                 },
                 {'name':'About Me',
                 'anchor':'#About',
                 },
                 {'name':'My Skills',
                 'anchor':'#Skills',
                 },
                 {'name':'My Projects',
                 'anchor':'#MyProjects',
                 },
                 {'name':'My Contacts',
                 'anchor':'#MyContacts',
                 },
        ]
        }
        
    },  
}

</script>

<template>
   <header class="animate__animated animate__fadeInDown mb-5 fixed-top ">
    <nav class="navbar navbar-expand-lg navbar-dark  " aria-label="Fifth navbar example">
    <div class="container-fluid">
      <img class="logo_portfolio rounded-5" src="../assets/logo.png" alt="">
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarsExample05" aria-controls="navbarsExample05" aria-expanded="true" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="navbar-collapse collapse show " id="navbarsExample05" style="">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item" v-for="link in links">
            <a class="nav-link item" :href =' link.anchor '>{{link.name}}</a>
          </li>
        </ul>
     </div>
    </div>
  </nav>
    
   </header>
  

   <div class="'container-fluid  p-relative jumbo_hero mb-5" id="Home">
   
    
     
      <div class="px-4 py-5 text-center my-5 animate__animated animate__fadeInDown bg-black p-2  rounded-1" id="hero_container" >
        <p class="ele_ment">Salve mi chiamo Yari </p>
        <div class="col-lg mx-auto">
          <p class="mb-4  w-100 ele_ment" id="element" ></p>
       
      </div>
      
      </div>
   </div>
   
</template>

<style lang="scss">
header{
  border: 1px solid white;
  background-color: rgba($color: #000000, $alpha: 0.5);
  backdrop-filter: blur(4px);
  margin: 0 auto;
}

.item{
  transition: 3s;
}
.logo_portfolio{
    max-width: 50px;
}
@keyframes swing {
    0% {
      transform: rotate(0deg);
    }
    10% {
      transform: rotate(10deg);
    }
    20% {
      transform: rotate(-10deg);
    }
    30% {
      transform: rotate(6deg);
    }
    40% {
      transform: rotate(-6deg);
    }
    50% {
      transform: rotate(3deg);
    }
    60% {
      transform: rotate(-3deg);
    }
    70% {
      transform: rotate(2deg);
    }
    80% {
      transform: rotate(-2deg);
    }
    90% {
      transform: rotate(1deg);
    }
    100% {
      transform: rotate(0deg);
    }
  }
  
.nav_link:hover {
    display: inline-block;
    
  
    animation: swing; /* referring directly to the animation's @keyframe declaration */
    animation-duration: 2s; /* don't forget to set a duration! */
  }
  ul:hover li a {
    color: #30edf4;
  }
  
  ul:hover li a:not(:hover) {
    color: white;
    opacity: 0.3;
    filter: blur(1px);
  }
  
  
  .jumbo_hero{
    display: flex;
    justify-content: center;
    width: 100vw;
    min-height: 78vh;
    
   
  }
  
  .ele_ment{
    font-size: 15px;
    font-family: 'Anonymous Pro', monospace;
   
    
  }


  #hero_container{
    position: relative;
    color: #09d99a;
    align-self: center;
    border: 10px solid whitesmoke;
    min-width: 420px;
   
   
   
  }
 
  

</style>