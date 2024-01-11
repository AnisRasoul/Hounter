<template>
  <div class="about mt-5">
     <div class="text-center">
        <img src="../../assets/about/Group 10.png">
        <h2 class="mt-2">Find Out More About <br> Selling And Buying Homes</h2>
        <button class="navbtn mt-4" style="background-color:#10B981 ;">More Artikel</button>
     </div>
     <div class="container">
     <div class="row mt-5">
        <div class="col-sm-10 col-md-6">
           <div class="d-flex">
            <img src="../../assets/about/Dianne-villa.png" alt="">
            <div d-block class="ms-3">
                <img src="../../assets/about/dianne.svg" alt=""> 
                <h5> The things we need to check when we want to buy a house</h5>
                <div class="d-flex"><img src="../../assets/about/clock.svg" ><span class="ms-3">4 min read | 25 Apr 2021</span> </div>
            </div>
           </div>
           <div class="d-flex mt-5">
            <img src="../../assets/about/Courtney-villa.png" alt="">
            <div d-block class="ms-3">
                <img src="../../assets/about/courtney.svg"  alt=""> 
                <h5> 7 Ways to distinguish the quality of the house we want to buy</h5>
                <div class="d-flex blog"><img src="../../assets/about/clock.svg"><span class="ms-3">4 min read | 25 Apr 2021</span> </div>
            </div>
           </div>
           <div class="d-flex mt-5">
            <img src="../../assets/about/Darlene-villa.png"  alt="">
            <div d-block class="ms-3">
                <img src="../../assets/about/darlene.svg" alt=""> 
                <h5> The best way to know the quality of the house we want to buy</h5>
                <div class="d-flex blog"><img src="../../assets/about/clock.svg"><span class="ms-3">4 min read | 25 Apr 2021</span> </div>
            </div>
           </div>
        </div>
        <div class=" col-sm-12 col-md-4 ms-5 mt-5">
                <img src="../../assets/about/Cameron-villa.png" id="cameron">
                <div class="d-flex mt-2">
                <img src="../../assets/about/Frame 19.svg" alt="">
                </div>
                <h2>12 Things to know before buying a house</h2>
                <h5>Want to buy a house but are unsure about what we should know, here I will try to explain what we should know and check when we want to buy a house</h5>
               <div class="d-flex">
                <img src="../../assets/about/clock.svg"> <span class="ms-3">8 min read | 25 Apr 2021</span>
               </div>
        </div>
     </div>
     </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
    .about{
        background-image: url('../../assets/about/topblur.png'), url('../../assets/about/midblur.png');
        overflow-x: hidden;
        font-family:'Lexend';
        background-position: 0% 100%, 0% 0%;
        background-repeat: no-repeat;
        background-size:38%;
        color: #1B1C57;
        font-weight: 600;
    }
    @media (max-width: 800px) {
        .about{
            background-size:100% ;
        }
        .container{
            margin-left:0% ;
        }
        .d-flex h5 {
      font-size: 14px;
      max-width: 40%;
    }
        .d-flex span {
      font-size: 12px;
      
    }
        #blog{
        height: auto;
        width: 10%;
    }
        #cameron{
        height: auto;
        width: 80%;
    }
         h2{
        max-width: 80%;
    }
        h5{
        max-width: 60%;
        font-size: 18px;
    }

    }
</style>
