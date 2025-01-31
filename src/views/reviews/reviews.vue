<template>
  <div class="reviews">
    <div class="text-center mb-5">
      <span><img src="../../assets/reviews/Group 10.png" alt="" /></span>
      <h1>What Our User Say About Us</h1>
    </div>

    <div class="swiper-container">
      <div class="swiper-wrapper">
        <div class="swiper-slide">
          <img src="../../assets/reviews/Review.png" />
        </div>
        <div class="swiper-slide">
          <img src="../../assets/reviews/Review-3.png" />
        </div>
        <div class="swiper-slide">
          <img src="../../assets/reviews/Review-4.png" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Swiper from "swiper";
import "swiper/swiper-bundle.css";

export default {
  mounted() {
    var mySwiper = new Swiper(".swiper-container", {
      loop: true,
      slidesPerView: 1, // Show one slide per view
    });
  },
};
</script>

<style scoped>
.reviews {
  overflow-x: hidden;
  color: #1b1c57;
}
.swiper-container {
  width: 50%;
  height: 700px;
}
@media (max-width: 800px) {
  .swiper-container {
    width: 100%;
    height: auto; /* Adjust height as needed */
  }

  .swiper-slide img {
    width: 95%; /* Make images fill their container */
    height: auto; /* Maintain aspect ratio */
  }
}
</style>
