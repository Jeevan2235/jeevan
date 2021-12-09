<template>
  <div>
  <div>
    <h1 class="mt-8">Apartment Overview</h1>
    <v-row>
      <v-card
        v-for="n in 2"
        :key="n"
        class="pa-7 mt-10 ma-2"
        outlined
        height="2em"
        width="20em"
        style="font-weight: bold; background-color: #f8f8f8"
      >
        <v-row>
          <p>Deposit / Bond</p>
          <v-spacer></v-spacer>
          <p>$225000.00</p>
        </v-row>
      </v-card>
    </v-row>
    <v-row>
      <v-card
        v-for="n in 2"
        :key="n"
        class="pa-7 mt-3 ma-2"
        outlined
        height="2em"
        width="20em"
        style="font-weight: bold; background-color: #f8f8f8"
      >
        <v-row>
          <p>Total Area (sq. ft)</p>
          <v-spacer></v-spacer>
          <p>300</p>
        </v-row>
      </v-card>
    </v-row>
    <v-row>
      <v-card
        v-for="n in 2"
        :key="n"
        class="pa-7 mt-3 ma-2"
        outlined
        height="2em"
        width="20em"
        style="font-weight: bold; background-color: #f8f8f8"
      >
        <v-row>
          <p>Car Parking Per Space</p>
          <v-spacer></v-spacer>
          <p>02</p>
        </v-row>
      </v-card>
    </v-row>
    <v-row>
      <v-card
        v-for="n in 2"
        :key="n"
        class="pa-7 mt-3 ma-2"
        outlined
        height="2em"
        width="20em"
        style="font-weight: bold; background-color: #f8f8f8"
      >
        <v-row>
          <p>Air Condition</p>
          <v-spacer></v-spacer>
          <p>02</p>
        </v-row>
      </v-card>
    </v-row>

    <!-- <v-row>
      <v-card
        class="pa-7 mt-3 ma-2"
        outlined
        height="4em"
        width="20em"
        tile
        style="background-color: #f8f8f8"
      > -->
        <!-- <v-row>
          <h2>Indoor features:</h2>
        </v-row>
        <v-col>
          <div class="mt-7">
            <p style="font-weight: bold; color: #66666f">-- Community Hall</p>
            <p style="font-weight: bold; color: #66666f">-- Safety Grills</p>
            <p style="font-weight: bold; color: #66666f">-- Servants Room</p>
            <p style="font-weight: bold; color: #66666f">-- Servants Toilet</p>
            <p style="font-weight: bold; color: #66666f">-- Fire exit</p>
            <p style="font-weight: bold; color: #66666f">-- CCTV</p>
            <p style="font-weight: bold; color: #66666f">-- WASA connection</p>
            <p style="font-weight: bold; color: #66666f">-- DESCO connection</p>
            <p style="font-weight: bold; color: #66666f">
              -- TITAS GAS connection
            </p>
            <p style="font-weight: bold; color: #66666f">-- Balcony</p>
            <p style="font-weight: bold; color: #66666f">-- Inter Com</p>
          </div>
        </v-col>
      </v-card>

       <v-card
        class="pa-7 mt-3 ma-2"
        outlined
        height="4em"
        width="20em"
        tile
        style="background-color: #f8f8f8"
      >
        <v-row>
          <h2>Indoor features:</h2>
        </v-row>
        <div class="mt-7">
          <v-col>
            <p style="font-weight: bold; color: #66666f">-- South facing</p>
            <p style="font-weight: bold; color: #66666f">-- Roof Top Garden</p>
            <p style="font-weight: bold; color: #66666f">-- Drivers quarters</p>
            <p style="font-weight: bold; color: #66666f">-- Generator</p>
            <p style="font-weight: bold; color: #66666f">-- Lift</p>
          </v-col>
        </div>
      </v-card> 
    </v-row> -->
  </div>
  </div>
</template>

<script>
export default {

};
</script>

<style>
</style>