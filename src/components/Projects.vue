<template>
  <v-container class="px-0 my-14">
    <h3 class="mb-4 text-h5 blac--text">Projects</h3>
    <v-divider></v-divider>
    <v-container fluid class="pa-0 mt-10">
      <v-row dense class="ma-0">
        <v-col v-for="card in cards" :key="card.title" cols="3" class="">
          <Card :title="card.title" :imgSrc="card.imgSrc"  />
        </v-col>
      </v-row>
    </v-container>
  </v-container>
</template>

<script>
import Card from "./Card.vue";
export default {
  components: {
    Card,
  },
  data() {
    return {
      cards: [
        { title: "Summer House", imgSrc: 'https://www.w3schools.com/w3images/house5.jpg' },
        { title: "Brick House", imgSrc: 'https://www.w3schools.com/w3images/house2.jpg' },
        { title: "Renovated", imgSrc: 'https://www.w3schools.com/w3images/house3.jpg' },
        { title: "Barn House", imgSrc: 'https://www.w3schools.com/w3images/house4.jpg' },
        { title: "Summer House", imgSrc: 'https://www.w3schools.com/w3images/house2.jpg' },
        { title: "Brick House", imgSrc: 'https://www.w3schools.com/w3images/house5.jpg' },
        { title: "Renovated", imgSrc: 'https://www.w3schools.com/w3images/house4.jpg' },
        { title: "Barn House", imgSrc: 'https://www.w3schools.com/w3images/house3.jpg' },
      
      ],
    };
  },
};
</script>


<style scoped>
</style>