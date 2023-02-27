<script>
    export default{
    data() {
        return {
          
            slides:[

                     {"image":"dadi.png",
                      "name":"Dadi",
                     "paragraph": "Gioco dadi" ,},

                     {"image":"MaxCoach.png",
                      "name":"Distant Learning",
                     "paragraph": "Sito ispirato ad una scuola che insegna da remoto" ,},

                     {"image":"spotify.png",
                      "name":"Spotify",
                     "paragraph": "Web App Ispirata a Spotify" ,},

                     {"image":"Discord.png",
                      "name":"Discord",
                     "paragraph": "Sito ispirato a Discord" ,},

        ]
        }
    },
 }


</script>

<template>

<section id="MyProjects">
    <h2 class="text-center text-white">
        My projects
    </h2>
    <div id="github_link">
      Questi sono alcuni dei miei progetti. <br> Per visionarne  altri  guarda il mio profilo <a class="text-decoration-none "  href="https://github.com/Knil88">Github</a>
    </div>
    <div id="carouselExampleAutoplaying" class="carousel slide " data-bs-ride="carousel">
      <div class="carousel-inner">
       
        <div class="carousel-item   active  p-relative ">
          <img src="boolflix.png" class="d-block w-75 m-auto" alt="...">
          <div class="carousel_title text-center carousel-caption d-none d-md-block">
            Gioco dei Dadi :
            <p>
              Gioco Dadi con lancio casuale
            </p>
          </div>
        </div>
        <div class="carousel-item p-relative">
          <img src="spotify.png" class="d-block w-75 m-auto" alt="...">
          <div class="carousel_title text-center carousel-caption d-none d-md-block">
            Spotify:
            <p>
              Sito ispirato a Spotify
            </p>
          </div>
        </div>
        <div class="carousel-item p-relative ">
          <img src="MaxCoach.png" class="d-block w-75 m-auto" alt="...">
          <div class="carousel_title text-center carousel-caption d-none d-md-block">
           Distant Learning:
            <p>
              Sito ispirato di corsi online 
            </p>
          </div>
        </div>
      
      </div>
      <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleAutoplaying" data-bs-slide="prev">
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Previous</span>
      </button>
      <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleAutoplaying" data-bs-slide="next">
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Next</span>
      </button>
    </div>
   
  


</section>
        
    
</template>

<style lang="scss">
.carousel-item{
  min-height: 230px;
}
.carousel_title{
    color: #09d99a;
    border: 10px solid rgb(100, 18, 18);
    background-color: black;
    font-family: 'Anonymous Pro', monospace;
    padding: 15px;
    font-size: 14px;
    max-width: 300px;
    margin: auto;
    
   
    
    
  }
 
  #nxt,#prw{
    width: 30%;
  }
  #github_link{
    color: #09d99a;
    border: 10px solid rgb(236, 217, 217);
    background-color: black;
    font-family: 'Anonymous Pro', monospace;
    padding: 15px;
    font-size: 14px;
    max-width: 500px ;
    margin: 20px auto;
  }
  
</style>