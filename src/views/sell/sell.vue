<template>
   <div class="sell">
    <div class="container animate__animated animate__slideInLeft animate__delay-5s">

    <span><img src="../../assets/sell/Group 11.png" alt=""></span>
    <div class="row mb-5 mt-2" style="font-family: 'Lexend'; font-weight:600 ;color:#1B1C57">
        <div class="col-sm-12 col-md-6 mt-5 ">
            <h1 style="font-weight: 800; max-width: 95%;">Let’s tour and see our house!</h1>
            <p class="mt-1" style="font-weight: 200; font-size:18px; max-width: 60%;">Houses recommended by our partners that have been curated to become the home of your dreams!</p>
            <h5 style="font-weight: 600;">House Detail</h5>
            <div class="house-detail mt-2">
                <p class="me-5"><img class="me-2" src="../../assets/sell/bed.svg"> 4 Bedroom</p>  <p class="ms-5 me-5"><img class="me-2" src="../../assets/sell/bathroom.svg">2 Bathrooms</p>
            </div>
            <div class="house-detail mt-3">
                <p class="me-5 "><img class="me-2" src="../../assets/sell/carport.svg"> 1 Carport</p>  <p class="ms-5 me-5"><img class="me-2 ms-2" src="../../assets/sell/floors.svg">2    Floors</p>
            </div>
            <div class="house-detail mt-4">
                <span><img id="dianne" src="../../assets/recommendation/dianne.svg"></span> <button class="sellbtn"><img src="../../assets/sell/phone.svg">Contact now</button>
            </div>
        </div>
        <div class="col-sm-12 col-md-6">
            <img class="img-fluid" src="../../assets/sell/houses.svg">
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
    
    .sell{
        
        overflow-x: hidden;
        font-family:'Lexend';
        background-image:url('../../assets/sell/blur.png'), url('../../assets/sell/blue2.png');
        background-position: 100% 50%;
        background-repeat: no-repeat;
        background-size:36%;
        
    }
    .sellbtn{
    outline: 0;
    border: 0;
    cursor: pointer;
    border-radius: 50px;
    padding: 8px 16px;
    font-size: 16px;
    background-color:#10B981 ;
    font-weight: 700;
    color: white;
    line-height: 26px; 
    }
    .container{
margin-left: 17% ;
    }
    .house-detail{
        display: flex;   
    }
    @media (max-width: 800px) {
        .sell{
            background-size: cover ;
        }
        .container{
            margin-left:0% ;
        }
        #dianne{
      height: 35px; /* Set the height as needed */
    }
    .sellbtn {
      padding: 6px 12px; /* Adjust padding to match the height of the dianne.svg */
      font-size: 14px; /* Modify font size to match the size of the text in dianne.svg */
    }
    .sellbtn img {
      height: 16px; /* Set the height to your preferred size */
      margin-right: 6px; /* Add margin for better spacing if needed */
    }
        
        
    }
</style>