<template>
  <div class="mt-16" style="background-color: #ffffff">
    <v-row>
      <v-col col="12" md="2.5" sd="6" v-for="thing in things" :key="thing">
        <v-img :src="thing.img" height="20em"> </v-img>
        <v-img class="mt-2" :src="thing.img" height="20em"> </v-img>
      </v-col>
      <v-col cols="12" md="4" sd="6">
        <h1
          style="
            font-size: 70px;
            font-family: Playfair Display, serif;
            color: #0e385d;
          "
        >
          Our <br />Photo <br />Gallery
        </h1>
        <p style="font-weight: bold; font-size: 25px; color: #66666f">
          Best of our <br />Event portfolio Photos
        </p>
        <p>
          Amorem ipsum dolor sit amet, consectetur adipiscing elit. Cras vitae
          nibh nisl. Cras etitikis mauris eget lorem ultricies ferme ntum a inti
          diam. Morbi mollis pellen tesque offs aiug ueia nec rhoncus. Nam
          <br />ute ultricies.
        </p>
        <v-btn
          rounded
          class="white--text mt-5 mb-16"
          height="50"
          width="230"
          color="#0e385d"
          >All photos & videos</v-btn
        >
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  data: () => ({
    things: [
      {
        img: "man.png",
      },
      {
        img: "car.png",
      },
      {
        img: "snow.png",
      },
    ],

   
  }),
};
</script>

<style></style>
