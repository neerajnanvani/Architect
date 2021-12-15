<template>
    <v-card>
        <v-app-bar absolute color="white" elevatation="4" height = "55">
      <v-btn  id="logo-btn" text color="black" class="font-weight-regular text-capitalize"
        ><span class="font-weight-black mr-1">BR</span>Architects</v-btn
      >

      <v-spacer></v-spacer>

    <div>
        <v-btn v-for="btn in buttons" :key="btn" id="logo-btn" text class="black--text font-weight-medium text-capitalize">
            {{btn}}
        </v-btn>
    </div>
   
    </v-app-bar>
    </v-card>
</template>

<script>

export default{
    data(){
        return{
            buttons:['Projects', 'About', 'Contact']
        }
    }
};
</script>

<style scoped>

#logo-btn{
  letter-spacing: 4px !important;
  font-family: Verdana, sans-serif !important;
  font-size: 15px;
  color: #000000;
}
</style>