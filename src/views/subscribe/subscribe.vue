<template>
  <div class="container">
<div class="subscribe text-center align-items-center justify-content-center">
  <h1 style="color:#1B1C57 ;">Subscribe for more info <br> And Update From Hunter</h1>
  <div class="wrapper ">
    <input type="text" placeholder="Your email here">
    <button style="background-color:#10B981 ; color:white">Subscribe here!</button>
  </div>
</div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
 .subscribe{
  background-image: url('../../assets/subscribe/Subscribe.png');
  background-repeat: no-repeat ;
  background-size:100%; 
  padding: 8%;
  
  
 }
.wrapper input {
  border: 2px solid rgb(181, 181, 181);
  border-radius: 50px ;
  padding: 10px;
 
}

@media (max-width: 800px) {
    .subscribe{
     background-image: none;
     padding: 0%;
    }
}


</style>