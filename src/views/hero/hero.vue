<template>

    <div class="hero">
      <div class="container">

     <nav class="navbar navbar-expand-md navbar-light">
        <div class="container-fluid d-flex justify-content-between align-items-center">
          <a class="navbar-brand " style=";" href="#intro">
            <img src="../../assets/hero/Logo.png" >
          </a>
          <button class="navbar-toggler d-lg-none" type="button" data-bs-toggle="collapse" data-bs-target="#collapsibleNavId" aria-controls="collapsibleNavId"
                aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse " id="collapsibleNavId">
          <ul class="navbar-nav text-center ms-auto">
            <li class="nav-item">
                <button type="button" class="navbtn mx-3 mt-2">About</button>
            </li>
            <li class="nav-item">
                <button type="button" class="navbtn mx-3 mt-2">Article</button>
             </li>
           
            <li class="nav-item">
              <div class="dropdown">
              <button class="navbtn mx-3 mt-2 dropdown-toggle" type="button" id="dropdownMenuButton1" data-bs-toggle="dropdown" aria-expanded="false">Property</button>
                  <ul class="dropdown-menu mt-2 ms-3" aria-labelledby="dropdownMenuButton1">
                  <li><a class="dropdown-item" href="#">Villa</a></li>
                  <li><a class="dropdown-item" href="#">Appartment</a></li>
                  <li><a class="dropdown-item" href="#">House</a></li>
                 </ul>
              </div>
            </li>
            
            <li class="nav-item">
                <button type="button" class="navbtn mx-5 mt-2" style="background-color:#D1FAE5 ;">SignUp!</button>
            </li>
          </ul>
        </div>
        </div>
      </nav>
   
  <div class="row mt-4 " style="font-family: 'Lexend'; font-weight:600; color:#1B1C57;">
    <div class="col-sm-10 col-md-6">
      <h1 class="display-3 header" style="max-width: 80%; font-weight: 800;">Find the place to live <span class="outline-text">your dreams</span> easily here</h1>
      <p class="mt-3 header" >Everything you need about finding your place to live will be here, where it will be easier for you</p>
      <div class="custom-search">
  <input type="text" class="custom-search-input" placeholder="Search for the location you want!">
  <button class="custom-search-botton" type="submit">Search</button>  
    </div> 
    <p class="mt-3">Our Partnership</p>
    <img class="partners" src="../../assets/hero/Partnership.png">
    </div>
    <div class="col">
      <div class="swiper-container sc" style="width: 18vw;">
          <div class="swiper-wrapper">
            <div class="swiper-slide"><img src="../../assets/hero/1K Peoples.png"></div>
            <div class="swiper-slide"><img src="../../assets/hero/56houses.png"></div>
            <!-- Add more slides as needed -->
    </div>
      </div>
    </div>
   
  </div>
      </div>
</div>
   
   
</template>

<script>
import Swiper from 'swiper';
import 'swiper/swiper-bundle.css';
export default {
  mounted() {
     
     var mySwiper = new Swiper('.swiper-container', {
       loop: true,
     });
   },
  
}
</script>

<style>
  .hero{
    background-image: url('../../assets/hero/Color Blur.png'), url('../../assets/hero/villa.png');
    background-position:top left, top right ;
    background-repeat: no-repeat;
    background-size:contain, 45%;
    max-width: 100%;
    overflow-x: hidden;
    height: 100%;
  }
  .container{
    margin-left: 17%;
  }
    .custom-search {
  position: relative;
  width: 400px;
}
.custom-search-input {
  width: 126%;
  border: 1px solid #ccc;
  border-radius: 100px;
  padding: 15px 100px 20px 20px; 
  line-height: 1;
  box-sizing: border-box;
  outline: none;
}
.custom-search-botton {
  position: absolute;
  margin-left:405px ;
  top: 3px;
  bottom: 3px;
  border: 0;
 background: #10B981;
  color: #fff;
  outline: none;
  
  padding: 0 20px;
  border-radius: 100px;
  z-index: 2;
}
.navbtn{ 
outline: 0;
border: 0;
cursor: pointer;
background-color:#d1fae52f ;
border-radius: 50px;
padding: 8px 16px;
font-size: 16px;
font-weight: 700;
color: white;
line-height: 26px;                
}
.outline-text{
  color: rgba(255, 255, 255, 0.921);
  text-shadow: -1px -1px 0 #1B1C57,  
               1px -1px 0 #1B1C57,  
               -1px 1px 0 #1B1C57,  
               1px 1px 0 #1B1C57;
}
  .dropdown-menu{
  background-color: rgba(255, 255, 255, 0.298); 
  }
  .sc {
    margin-top: 40%;
    margin-left: 25% ;
  }
  .header{
    -webkit-animation: text-focus-in 2s cubic-bezier(0.550, 0.085, 0.680, 0.530) both;
	        animation: text-focus-in 2s cubic-bezier(0.550, 0.085, 0.680, 0.530) both;
  }
  @-webkit-keyframes text-focus-in {
  0% {
    -webkit-filter: blur(12px);
            filter: blur(12px);
    opacity: 0;
  }
  100% {
    -webkit-filter: blur(0px);
            filter: blur(0px);
    opacity: 1;
  }
}
@keyframes text-focus-in {
  0% {
    -webkit-filter: blur(12px);
            filter: blur(12px);
    opacity: 0;
  }
  100% {
    -webkit-filter: blur(0px);
            filter: blur(0px);
    opacity: 1;
  }
}
  @media (max-width: 800px) {
    .sc {
      display: none;
    }
    .custom-search-input {
      width: 50%; 
      padding: 10px 10px; 
      margin-right: 0; 
    }

    .custom-search-botton {
      margin-left: 0px; 
    }
    .navbtn {
      background-color: #1B1C57; 
      margin-top: 10px; 
    }
    .hero {
      background-image: url('../../assets/hero/Color Blur.png');
      background-position: top;
      background-repeat: no-repeat;
      background-size: top;
      max-width: 100%;
      overflow-x: hidden; 
    }
    .container{
      margin-left:0% ;
    }
    .hero::before {
      display: none;
    }
    .partners {
      max-width: 80%; 
      height: auto; 
    }
  }

 


   
</style>