<template>
    <div class="card mt-3 border-0 fw-lighter" style="width: 20rem;">
      <img :src="cardImage" class="card-img-top" alt="Card Image">
      <div class="card-body">
        <h4 class="card-title">{{ cardDesc }}</h4>
        <p class="card-text">{{ cardPrice }}</p>
        <img :src="authorImage" alt="Author Image" class="author-image">
      </div>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      cardImage: String,
      cardDesc: String,
      cardPrice: String,
      authorImage: String 
     
    }
  }
  </script>

<style>

</style>