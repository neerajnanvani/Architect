<template>
  <v-container class="px-0 my-14 my_container">
    <h3 class="text-h5 black--text">Projects</h3>
    <v-divider class="header_divider"></v-divider>
    <v-container fluid class="pa-0 mt-10">
      <v-row dense class="row">
        <v-col v-for="card in cards" :key="card.title" cols="3" class="col mb-4">
          <Card :title="card.title" :imgSrc="card.imgSrc" />
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
        {
          title: "Summer House",
          imgSrc: "https://www.w3schools.com/w3images/house5.jpg",
        },
        {
          title: "Brick House",
          imgSrc: "https://www.w3schools.com/w3images/house2.jpg",
        },
        {
          title: "Renovated",
          imgSrc: "https://www.w3schools.com/w3images/house3.jpg",
        },
        {
          title: "Barn House",
          imgSrc: "https://www.w3schools.com/w3images/house4.jpg",
        },
        {
          title: "Summer House",
          imgSrc: "https://www.w3schools.com/w3images/house2.jpg",
        },
        {
          title: "Brick House",
          imgSrc: "https://www.w3schools.com/w3images/house5.jpg",
        },
        {
          title: "Renovated",
          imgSrc: "https://www.w3schools.com/w3images/house4.jpg",
        },
        {
          title: "Barn House",
          imgSrc: "https://www.w3schools.com/w3images/house3.jpg",
        },
      ],
    };
  },
};
</script>


<style scoped>
.my_container {
  max-width: 1564px !important;
  margin: 0px 170.5px !important;
  padding: 8px 16px !important;
}

.my_container h3 {
  padding: 48px 16px 20px 16px !important;
}

.my_container .row {
  padding: 0px 8px !important;
}
.my_container .header_divider {
  border-width: 1px 10px !important;
  margin: auto;
}

.my_container .col {
  padding: 0px 8px !important;
}
</style>