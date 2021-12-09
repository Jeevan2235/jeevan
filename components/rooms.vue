<template>
  <div class="ml-16">
    <v-container>
      <h1
        class="text-center"
        style="
          font-size: 60px;
          font-family: Playfair Display, serif;
          color: #0e385d;
        "
      >
        Rooms & Apartments
      </h1>
      <h3 class="text-center" style="font-size: 16px; color: #0e385d">
        FIND YOUR ROOMS, FOR YOUR ABAILITY
      </h3>
      <v-row>
        <div v-for="link in links" :key="link">
          <v-card elevation="0" width="370px" class="mt-5">
            <v-card class="pa-4" elevation="0" color="#f7f7f7">
              <v-card elevation="0">
                <v-img :src="link.img" height="250"> </v-img>

                <v-card-title>{{ link.title }}</v-card-title>

                <v-card-text class="text-subtitle-1"
                  ><v-icon>mdi-map-marker</v-icon>Dhanmodia, Dhaka
                </v-card-text>

                <v-divider class="mx-4"></v-divider>

                <v-card-text class="text-subtitle-1 mx-2"
                  ><v-icon>mdi-bed</v-icon>{{ link.bedroom }}
                  <v-icon class="pl-3">mdi-bathtub</v-icon>
                  {{ link.bathroom }}</v-card-text
                >
                <v-card-title class="font-bold"
                  >$200
                  <v-spacer></v-spacer>
                  <v-icon>mdi-share-variant </v-icon
                  ><v-icon class="ml-2">mdi-star-outline</v-icon>
                </v-card-title>
              </v-card>
            </v-card>
          </v-card>
        </div>
      </v-row>

      <div class="text-center">
        <v-btn
          rounded
          color="#0e385d"
          elevation="0"
          class="white--text mt-5"
          height="50"
          width="200"
          >All Apartments</v-btn
        >
      </div>
    </v-container>
  </div>
</template>

<script>
export default {
  data: () => ({
    links: [
      {
        img: "building.jpg",
        title: "Family Apartment",
        address: "Dhanmondi, Dhaka",
        bedroom: "3 Bedrooms",
        bathroom: "2 Bathroom",
        price: "$200",
      },
      {
        img: "building.jpg",
        title: "Family Apartment",
        Address: "Dhanmondi, Dhaka",
        bedroom: "3 Bedrooms",
        bathroom: "2 Bathroom",
        Price: "$200",
      },
      {
        img: "building.jpg",
        title: "Family Apartment",
        Address: "Dhanmondi, Dhaka",
        bedroom: "3 Bedrooms",
        bathroom: "2 Bathroom",
        Price: "$200",
      },
      {
        img: "building.jpg",
        title: "Family Apartment",
        Address: "Dhanmondi, Dhaka",
        bedroom: "3 Bedrooms",
        bathroom: "2 Bathroom",
        Price: "$200",
      },
      {
        img: "building.jpg",
        title: "Family Apartment",
        Address: "Dhanmondi, Dhaka",
        bedroom: "3 Bedrooms",
        bathroom: "2 Bathroom",
        Price: "$200",
      },
      {
        img: "building.jpg",
        title: "Family Apartment",
        Address: "Dhanmondi, Dhaka",
        bedroom: "3 Bedrooms",
        bathroom: "2 Bathroom",
        Price: "$200",
      },
    ],
  }),
};
</script>

<style></style>
