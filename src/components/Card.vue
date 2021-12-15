<template>

  <v-container class="faltu_container pa-0">
    
    <v-img :src="imgSrc" class="meri_img ma-0"> </v-img>
    <span>{{ title }}</span>
  </v-container>
</template>

<script>
export default {
  props: ["title", "imgSrc"],
};
</script>

<style scoped>
.faltu_container{
    position: relative;
}
.faltu_container span {
  position: absolute !important;
  top: 0 !important;
  left: 0;
background:rgb(0, 0, 0);
padding:6px 12px;
color:white;
  font-weight: 400;
  font-size: 15px;
}

</style>