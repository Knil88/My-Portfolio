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
    

<div class="container conbg" id="conbg">
  <div class="bg2" id="bg2">
    <div class="bg1" id="bg1">
      <div class="bg  " id="bg" >
        <div class="bg-text text-light carousel_title ps-3">
          <h3>Dadi</h3>
          <p>
           Gioco Dadi
          </p>
          <a class="text-light" href="#bg1"><svg viewBox="0 0 448 512" width="30" fill="#fff" title="angle-double-right">
              <path d="M224.3 273l-136 136c-9.4 9.4-24.6 9.4-33.9 0l-22.6-22.6c-9.4-9.4-9.4-24.6 0-33.9l96.4-96.4-96.4-96.4c-9.4-9.4-9.4-24.6 0-33.9L54.3 103c9.4-9.4 24.6-9.4 33.9 0l136 136c9.5 9.4 9.5 24.6.1 34zm192-34l-136-136c-9.4-9.4-24.6-9.4-33.9 0l-22.6 22.6c-9.4 9.4-9.4 24.6 0 33.9l96.4 96.4-96.4 96.4c-9.4 9.4-9.4 24.6 0 33.9l22.6 22.6c9.4 9.4 24.6 9.4 33.9 0l136-136c9.4-9.2 9.4-24.4 0-33.8z" />
            </svg></a>
        </div>
      </div>
      <div class="bg-text text-light ps-3  carousel_title">
        <h3>Discord</h3>
        <p>
          Sito ispirato a Discord
        </p>
        <a class="text-light" href="#bg2"><svg viewBox="0 0 448 512" width="30" fill="#fff" title="angle-double-right">
            <path d="M224.3 273l-136 136c-9.4 9.4-24.6 9.4-33.9 0l-22.6-22.6c-9.4-9.4-9.4-24.6 0-33.9l96.4-96.4-96.4-96.4c-9.4-9.4-9.4-24.6 0-33.9L54.3 103c9.4-9.4 24.6-9.4 33.9 0l136 136c9.5 9.4 9.5 24.6.1 34zm192-34l-136-136c-9.4-9.4-24.6-9.4-33.9 0l-22.6 22.6c-9.4 9.4-9.4 24.6 0 33.9l96.4 96.4-96.4 96.4c-9.4 9.4-9.4 24.6 0 33.9l22.6 22.6c9.4 9.4 24.6 9.4 33.9 0l136-136c9.4-9.2 9.4-24.4 0-33.8z" />
          </svg></a>
      </div>
    </div>
    <div class="bg-text text-light ps-3  carousel_title">
      <h3>Spotify</h3>
      <p>
        Web App ispirata a Spotify
      </p>
      <a class="text-light" href="#conbg"><svg viewBox="0 0 448 512" width="30" fill="#fff" title="angle-double-right">
          <path d="M224.3 273l-136 136c-9.4 9.4-24.6 9.4-33.9 0l-22.6-22.6c-9.4-9.4-9.4-24.6 0-33.9l96.4-96.4-96.4-96.4c-9.4-9.4-9.4-24.6 0-33.9L54.3 103c9.4-9.4 24.6-9.4 33.9 0l136 136c9.5 9.4 9.5 24.6.1 34zm192-34l-136-136c-9.4-9.4-24.6-9.4-33.9 0l-22.6 22.6c-9.4 9.4-9.4 24.6 0 33.9l96.4 96.4-96.4 96.4c-9.4 9.4-9.4 24.6 0 33.9l22.6 22.6c9.4 9.4 24.6 9.4 33.9 0l136-136c9.4-9.2 9.4-24.4 0-33.8z" />
        </svg></a>
    </div>
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
  conbg {
  width: 100%;
  height: 500px;
}
.bg2 {
  z-index: 2;
  position: relative;
  width: 70%;
  margin: 100px auto;
  transform: rotate(10deg);
  background-image: url('spotify.png');
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
  background-image: url('Discord.png');
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
  background-image: url('dadi.png');
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


  
</style>