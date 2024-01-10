<template>
  <div class="home">
   <hero class="mb-5"></hero>
   <recommendation class="mb-5"></recommendation>
   <sell class="mb-5" ></sell>
   <reviews></reviews>
   <about class="mb-5"></about>
   <subscribe></subscribe>
   <foot ></foot>
  </div>
</template>

<script>
import hero from './hero/hero.vue'
import recommendation from './recommendation/recommendation.vue'
import sell from './sell/sell.vue'
import reviews from './reviews/reviews.vue'
import about from './about/about.vue'
import subscribe from './subscribe/subscribe.vue'
import foot from './footer/foot.vue'

export default {
  
  components: {
    hero,
    recommendation,
    sell,
    reviews,
    about,
    subscribe,
    foot,
    
  

  }
}
</script>

