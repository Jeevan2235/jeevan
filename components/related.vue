<template>
  <div class="mt-16" style="background-color:#f7f7f7">
      <h1 class="text-center" style="font-size:60px">Related apartments</h1>
    <v-container>
      <v-row>
          
        <div v-for="link in links" :key="link">
          <v-card elevation="0" width="360px" class="mt-5">
            <v-card class="pa-4" elevation="0" color="#f7f7f7">
              <v-card elevation="0" outlined>
                <v-img :src="link.img" height="250" > </v-img>

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
    </v-container>
  </div>
</template>


<script>
export default {
  data: () => ({
    links: [
      {
        img: "building.jpg",
        title: "Family Apasdcsdcdsc",
        address: "Dhanmondi, Dhaka",
        bedroom: "3 Bedrooms",
        bathroom: "2 Bathroom",
        price: "$200",
      },
      {
        img: "building.jpg",
        title: "Family",
        Address: "Dhanmondi, Dhaka",
        Bedroom: "3 Bedrooms, 2 Bathroom",
        Price: "$200",
      },
      {
        img: "building.jpg",
        title: "Family",
        Address: "Dhanmondi, Dhaka",
        Bedroom: "3 Bedrooms, 2 Bathroom",
        Price: "$200",
      },
    ],
  }),
};
</script>

<style>
</style>