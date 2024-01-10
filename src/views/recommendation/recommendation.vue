<template>
  <div class="recommendation">
    <span><img src="../../assets/recommendation/Group 10.png" alt=""></span>
    <div class="row mt-3">
        <div class="col-sm-2 col-md-3">
            <h1>Featured House</h1> 
        </div>
        <div class="col sm-10 col-md-9 mt-2">
            <button @click="showHouseCards" style="background-color:#D1FAE5; color:#10B981; outline: 1px solid #10B981;"><span><img src="../../assets/recommendation/house.svg" height="14px" class="mb-1 me-2"></span>House</button>
            <button @click="showVillaCards"><span><img src="../../assets/recommendation/villa.svg" height="14px" class="mb-1 me-2"></span>Villa</button> 
            <button @click="showApartmentCards"><span><img src="../../assets/recommendation/Appartment.svg" height="14px" class="mb-1 me-2"></span>Appartment</button> 
            <button><i class="fa-solid fa-chevron-left "></i></button> 
            <button><i class="fa-solid fa-chevron-right"></i></button> 
        </div> 
    </div>
    <div class="row mt-3">
      
    <card class="mx-auto" 
    v-for="card in filteredCards"
        :key="card.id"
        :card-image="card.cardImage"
        :card-desc="card.cardDesc"
        :card-price="card.cardPrice"
        :author-image="card.authorImage"
      
    />  
    </div>
    
  </div>
</template>

<script>
    import card from './card.vue'
export default {
    components: {
        card,
    },
    data() {
      return {
        cards: [
      { id: "1", cardImage:"https://i.imgur.com/m6zNa2M.png", cardDesc: "Roselands House", cardPrice: "$ 35.000.000", authorImage: "https://i.imgur.com/XyGcWhT.png" },
      { id: "2", cardImage:"https://i.imgur.com/0noTBCy.png", cardDesc: "Woodlandside", cardPrice: "$ 20.000.000", authorImage: "https://i.imgur.com/MuJdT0U.png" },
      { id: "3", cardImage:"https://i.imgur.com/xBA3Wnr.png", cardDesc: "The Old Lighthouse", cardPrice: "$ 44.000.000", authorImage: "https://i.imgur.com/Y8BlYcG.png" },
      { id: "4", cardImage:"https://i.pinimg.com/564x/4e/eb/f7/4eebf76e28e11ed1236436bde506a32b.jpg", cardDesc: "Los santos villa", cardPrice: "$ 60.000.000", authorImage: "https://i.imgur.com/Y8BlYcG.png" },
      { id: "5", cardImage:"https://i.pinimg.com/564x/37/a0/3f/37a03fa1fe6e4a034daf2d5994139a54.jpg", cardDesc: "New York villa", cardPrice: "$ 25.000.000", authorImage: "https://i.imgur.com/MuJdT0U.png" },
      { id: "6", cardImage:"https://i.pinimg.com/564x/7f/dd/c1/7fddc173fa462b5346f07c8a6155068e.jpg", cardDesc: "Chicago villa", cardPrice: "$ 25.000.000", authorImage: "https://i.imgur.com/XyGcWhT.png" },
      { id: "7", cardImage:"https://i.pinimg.com/564x/a9/8a/0a/a98a0ac85812d1f15585ad0d532dc177.jpg", cardDesc: "miami appartment", cardPrice: "$ 6.000.000", authorImage: "https://i.imgur.com/Y8BlYcG.png" },
      { id: "8", cardImage:"https://i.pinimg.com/564x/12/03/a5/1203a5b0a01f302d6b4a6f65216158a5.jpg", cardDesc: "vegas appartment", cardPrice: "$ 5.000.000", authorImage: "https://i.imgur.com/MuJdT0U.png" },
      { id: "9", cardImage:"https://i.pinimg.com/564x/60/22/d0/6022d07fc9bd655b14133901a6363cbd.jpg", cardDesc: "broklyn appartment", cardPrice: "$ 2.000.000", authorImage: "https://i.imgur.com/XyGcWhT.png" },
      
    ],
    filteredCards: []
    };
  },
  methods: {
    showHouseCards() {
      this.filteredCards = this.cards.filter(card => ['1', '2', '3'].includes(card.id));
    },
    showVillaCards() {
      this.filteredCards = this.cards.filter(card => ['4', '5', '6'].includes(card.id));
    },
    showApartmentCards() {
      this.filteredCards = this.cards.filter(card => ['7', '8', '9'].includes(card.id));
    }
    
  }
};



</script>

<style>
    .recommendation{
        margin-left: 17% ;
        overflow-x: hidden;
        font-family:'Lexend';
    }
    button{
outline: 1px solid #888B97;
border: 0;
cursor: pointer;
background-color: white ;
border-radius: 50px;
padding: 8px 16px;
font-size: 16px;
font-weight: 700;
color:#888B97;
line-height: 26px;  
margin-left: 2% ; 
    }
    @media (max-width: 800px){
      .recommendation{
      margin-left: 0% ;
        
      }
      button {
      font-size: 14px; /* Reduce font size for buttons on smaller screens */
      padding: 6px 12px; /* Adjust padding for buttons */
      margin: 4px; /* Adjust margin for buttons */
    }
    button i {
      font-size: 7px; /* Adjust the font size of the <i> elements for smaller screens */
    }  
    }
    
</style>