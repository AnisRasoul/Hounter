<template>
  <div class="foot">
    <br> <br>
    <div class="row footrow mt-5 mb-5">
        <div class="col-sm-12 col-md-3 me-5">
            <img src="../../assets/hero/Logo.png" alt="">
            <p class="mt-3">We provide information about properties such as houses, villas and apartments to help people find their dream home</p>
        
        <div class="d-flex mb-5">
            <a href="#" ><i class="fa-brands fa-facebook-f"></i></a>
            <a href="#" class="ms-5"><i class="fa-brands fa-twitter"></i></a>
            <a href="#" class="ms-5"><i class="fa-brands fa-instagram"></i></a> 
        </div>
    </div>
        
        <div class="col-sm-12 col-md-2 d-grid">
            <h2 class="header">Property</h2 >
            <a href="#">House</a>
            <a href="#">Apartment</a>
            <a href="#">Villa</a>
        </div>
        <div class="col-sm-12 col-md-2  d-grid">
            <h2 class="header">Article</h2 >
            <a href="#">New Article</a>
            <a href="#">Popular Article</a>
            <a href="#">Most Read</a>
            <a href="#">Tips & Tricks</a>
        </div>
        <div class="col d-grid contact">
            <h2 class="header">Contact</h2 >
            <span>2464 Royal Ln. Mesa, New Jersey 45463</span>
            <span>(671) 555-0110</span>
            <span>info@hounter.com</span>
            
        </div>
        <br><br>
    </div>
    <br><br>
   
  </div>
</template>

<script>
export default {

}
</script>

<style>
    .foot{
        overflow-x: hidden ;
        margin-bottom: auto;
        color: #1B1C57; 
        background-image: url('../../assets/foot/blue.png'),url('../../assets/foot/yellow.png');
        overflow-x: hidden;
        font-family:'Lexend';
        background-position: 100% calc(100% - 20px);
        background-repeat: no-repeat;
        background-size:60%,
        
        
        
    }
    .footrow{
        margin-left:17% ;
        margin-bottom: 50%;
    }
    i{
        font-size: 30px;
        color: #3C4563;
    }
    a{
        text-decoration: none;
        color: #3C4563;
    }
    .header{
        font-weight: 600;
    }
    @media (max-width: 800px) {
        .footrow{
            margin: 0%;
        }
        .foot{
            background-size: cover;
            background-position: center;
        }
}
</style>