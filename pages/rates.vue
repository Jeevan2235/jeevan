<template>
  <div>
    <h1
      class="text-center mt-16"
      style="
        font-size: 45px;
        color: #0e385d;
        font-family: Playfair Display, serif;"
    >
      For rates & Availability
    </h1>
    <h2 class="text-center " style="color: #0e385d">Search your House</h2>
    <div>
      <v-container>
        <v-row >
          <v-col cols="12" md="3" sm="4">
            <p class="pl-2">LIVING AREA</p>
            <v-text-field
            background-color="white"
            elevation="0"
              outlined
              label="Where do you want to live?"
              
              style="font-size: 12px; "
            ></v-text-field>
          </v-col>

          <v-col cols="12" md="2" sm="4">
            <p >TYPE</p>
            <v-select
            
            background-color="white"
          :items="items"
          label="Apartments"
          outlined
        ></v-select>
          </v-col>

          <v-col cols="12" md="2" sm="4">
            <p >PRICE</p>
            <v-text-field
            background-color="white"
              outlined
              label="Min"
              
            ></v-text-field>
          </v-col>

          <v-col cols="12" md="2" sm="4">
            <p >MALE</p>
            <v-text-field
            background-color="white"
              outlined
              label="Max"
              
            ></v-text-field>
          </v-col>

          <v-col cols="12" md="3" sm="4">
            <p >FOR</p>
            <v-select
            background-color="white"
          :items="items"
          label="Family"
          
           outlined
          
        ></v-select>
          </v-col>
        </v-row>
        <div class="text-center">
        <v-btn
          rounded
          color="#0e385d"
          elevation="0"
          class="white--text mt-5"
          height="50"
          width="200"
          >Check Availability</v-btn
        >
      </div>
      </v-container>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    items: ["Apartments", "Saab", "Mercedes", "Audi"],
    
    
  }),
};
</script>

<style>
</style>