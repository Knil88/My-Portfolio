<script>
    export default{
    data() {
        return {
          images:['spotify.png','MaxCoach.png','Discord.png']

        }
    },
 }


</script>

<template>

  <!-- Sezione Progetti -->

<section id="MyProjects">

    <h2 class="text-center text-white">

        My projects

    </h2>

    <div id="github_link">

      <!-- Richiamo link github -->

      Questi sono alcuni dei miei progetti. <br> Per visionarne  altri  guarda il mio profilo <a class="text-decoration-none "  href="https://github.com/Knil88">Github</a>

    </div>


    <div id="carouselExampleCaptions" class="carousel slide" data-bs-ride="false">

      <div class="carousel-inner responsive_carousel">
        <div class="carousel-item active">
          <img class="img-fluid " :src="images[0]" alt="" min-width="800" min-height="400">

          <div class="carousel-caption d-none d-md-block">
            <h5>First slide label</h5>
            <p>Some representative placeholder content for the first slide.</p>
          </div>
        </div>
        <div class="carousel-item">
          <img class="img-fluid " :src="images[1]" alt="" min-width="800" min-height="400">

          <div class="carousel-caption d-none d-md-block">
            <h5>Second slide label</h5>
            <p>Some representative placeholder content for the second slide.</p>
          </div>
        </div>
        <div class="carousel-item">
          <img class="img-fluid " :src="images[2]" alt="" min-width="800" min-height="400">

          <div class="carousel-caption d-none d-md-block">
            <h5>Third slide label</h5>
            <p>Some representative placeholder content for the third slide.</p>
          </div>
        </div>
      </div>
     <div class="responsive_button">
      <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="prev">
        <span class="carousel-control-prev-icon w-100" aria-hidden="true"></span>
        <span class="visually-hidden">Previous</span>
      </button>
      <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="next">
        <span class="carousel-control-next-icon w-100 " aria-hidden="true"></span>
        <span class="visually-hidden">Next</span>
      </button>
     </div>
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

background-color:rgba(0, 0, 0,0.7);

font-family: "Anonymous Pro", monospace;

padding: 15px;

  padding-left: 15px;

font-size: 14px;

width: 100%;

margin: auto;



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






.responsive_carousel{
  width: 75% !important;
  margin: auto;

}

.responsive_button{




  position: absolute;

height: 100px;
width: 85%;
bottom: 43%;
margin: auto 7%;
}

// Responsive
@media (max-width: 400px) {
  #github_link{
    max-width: 320px;
  }

  .responsive_carousel{
    width: 100% !important;


  }
 
}


</style>