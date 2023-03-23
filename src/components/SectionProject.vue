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
      <div class="carousel-indicators">
        <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
        <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="1" aria-label="Slide 2"></button>
        <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="2" aria-label="Slide 3"></button>
      </div>
      <div class="carousel-inner w-75 m-auto">
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
      <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="prev">
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Previous</span>
      </button>
      <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="next">
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

background-color:rgba(0, 0, 0,0.7);

font-family: "Anonymous Pro", monospace;

padding: 15px;

  padding-left: 15px;

font-size: 14px;

width: 100%;

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
  
.bg2 {

  z-index: 2;

  position: relative;

  width: 70%;
  
  margin: 100px auto;

  transform: rotate(10deg);
  
  background-image: url('https://media.licdn.com/dms/image/C4D2DAQGnEigTEzsfDA/profile-treasury-image-shrink_800_800/0/1678103538236?e=1678716000&v=beta&t=rUP2jaFOeFLBAL_5mua41AmRhs6jAO8AlScRVCtHEUE');

  background-size: contain;

  background-repeat:no-repeat;

  background-position: center;

  background-color: transparent;
  
}
.bg1 {

  z-index: 3;

  position: relative;

  margin: auto;

  transform: rotate(-5deg);

  background-image: url('https://media.licdn.com/dms/image/C4D2DAQF9Ee4FQajMjw/profile-treasury-image-shrink_800_800/0/1678103738771?e=1678716000&v=beta&t=X_8KTtM8SapqOOxU86VVXR7bF4uuinfTamK2dxUF08M');

  background-size: contain;

  background-repeat:no-repeat;

  background-position: center;

  background-color: transparent;
  
}

.bg {

  z-index: 4;

  position: relative;

  margin: auto;

  transform: rotate(-5deg);

  height: 500px;

  background-image: url('https://media.licdn.com/dms/image/C4D2DAQF_fJxnFgRwAA/profile-treasury-image-shrink_800_800/0/1678103602625?e=1678716000&v=beta&t=Ww-zZgL5_Fvbly06ZdZfIUAvk3Kr2NMGsUCODo94CKo');

  background-size: contain;

  background-repeat:no-repeat;

  background-position: center;

  background-color: transparent;
  
}
.bg-text {

  width: 100%;

  position: absolute;

  display: inline-block;

  bottom: 0;

  left: 0;

}
.bg-text a {

  margin: 5px;

  float: right;

}

#bg1:target .bg {

  animation: ciut 1s forwards;

}
#bg1:target {

  animation: fre 0.3s forwards;

}
#bg2:target .bg1 {
  animation: ciut 1s forwards;
}
#bg2:target {

  animation: fre1 0.3s forwards;

}
#conbg:target .bg2 {

  animation: ciut1 1s;

}
@keyframes fre1 {

  0% {

    transform: rotate(10deg);
  }
  100% {

    transform: rotate(0deg);

  }
}
@keyframes fre {

  0% {
    transform: rotate(-5deg);

  }
  100% {

    transform: rotate(-10deg);

  }
}
@keyframes ciut {

  0% {

    opacity: 1;

    transform: rotate(-5deg) scale(1);

  }
  100% {

    opacity: 0;

    transform: rotate(360deg) scale(0);

  }
}
@keyframes ciut1 {

  0% {

    opacity: 0;

    transform: rotate(0deg) scale(0);

  }
  100% {

    opacity: 1;

    transform: rotate(370deg) scale(1);
    
  }
}

// Responsive
@media (max-width: 400px) {
  #github_link{
    max-width: 320px;
  }
}
  
</style>