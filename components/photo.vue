<template>
  <div>
    <v-card height="35em" width="50em" v-for="thing in things" :key="thing">
      <v-img
        :src="thing.img"
        height="35em"
        width="50em"
        style="background-size: cover"
      ></v-img>
    </v-card>
    <v-row>
      <v-card v-for="link in links" :key="link" class="pa-2 mt-5" elevation="0" tile>
        <v-img :src="link.img1" height="6em" width="7em"> </v-img>
      </v-card>
    </v-row>
    <v-row>
      <h1 class="ml-2">Family Apartment</h1>
      <v-spacer></v-spacer>
      <p
        class="mr-16 pr-16 mt-2"
        style="color: #777a80; font-size: 20px; font-weight: bold"
      >
        Rent/Month: $550
      </p></v-row
    >
    <p class="mt-8" style="color: #777a80; font-size: 20px; font-weight: bold">
      3000 sq-ft., 3 Bedroom, Semi-furnished, Luxurious, South facing <br />
      Apartment for Rent in Rangs Malancha, Melbourne.
    </p>
  </div>
</template>

<script>
export default {
  data: () => ({
    things: [
      {
        img: "house2.png",
      },
    ],
    links: [
      {
        img1: "house2.png",
      },
      {
        img1: "about.png",
      },
      {
        img1: "building.jpg",
      },
      {
        img1: "car.png",
      },
      {
        img1: "bricks.png",
      },
      {
        img1: "sea.jpg",
      },
    ],
  }),
};
</script>

<style></style>
