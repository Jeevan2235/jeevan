<template>
  <div>
    <div style="background-color: #f7f7f7">
      <div
        class="text-center"
        style="
          background: linear-gradient(to right, #009933 20%, #333399 90%);
          height: 15em;
        "
      >
        <h1 class="pt-15 white--text" style="font-size: 45px">
          Choose Apartment
        </h1>
        <p style="font-weight: bold; font-size: 20px">
          Take A Apartment For Booking
        </p>
      </div>
    </div>

    <div style="background-color: #f7f7f7">
      <v-container>
        <h3 class="mb-16">
          Home > <span style="color: #999999">Apartment List For Booking</span>
        </h3>
        <v-row>
          <v-card
            v-for="popular in popular"
            :key="popular"
            color="#e8e8e8"
            elevation="0"
            height="4.5em"
            width="9em"
            class="text-center ma-2 mt-8"
          >
            <h3 class="mt-3">{{ popular.text }}</h3>
            <v-card-text style="margin-top: -20px">{{
              popular.text2
            }}</v-card-text>
          </v-card>

          <v-spacer></v-spacer>

          <v-select
            solo
            class="pr-7 mt-8"
            height="4em"
            :items="items"
            label="Category"
          >
          </v-select>
        </v-row>
        <div>
          <v-container>
            <v-row>
              <div v-for="thing in things" :key="thing">
                <v-card elevation="0" width="365px" class="mt-5 ma-2">
                  <v-img :src="thing.img" height="250"> </v-img>

                  <v-card-title>{{ thing.title }}</v-card-title>

                  <v-card-text class="text-subtitle-1"
                    ><v-icon>mdi-map-marker</v-icon>Dhanmodia, Dhaka
                  </v-card-text>

                  <v-divider class="mx-4"></v-divider>

                  <v-card-text class="text-subtitle-1 mx-2"
                    ><v-icon>mdi-bed</v-icon>{{ thing.bedroom }}
                    <v-icon class="pl-3">mdi-bathtub</v-icon>
                    {{ thing.bathroom }}</v-card-text
                  >
                  <v-card-title class="font-bold"
                    >$200
                    <v-spacer></v-spacer>
                    <v-icon>mdi-share-variant </v-icon
                    ><v-icon class="ml-2">mdi-star-outline</v-icon>
                  </v-card-title>
                </v-card>
              </div>
            </v-row>

            <div class="text-center">
              <v-btn
                class="white--text mt-15"
                color="#0e385d"
                height="45"
                width="150"
                >Load More</v-btn
              >
            </div>
          </v-container>
        </div>
      </v-container>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    links: ["Home", "Booking", "House", "Pages", "About", "Blog", "Contact"],

    items: ["Family", "Apartment", "Sublet", "Bachelor Mess", "Office"],

    popular: [
      {
        text: "Popular",
      },
      {
        text: "Date",
        text2: "Newest to Oldest",
      },
      {
        text: "Date",
        text2: "Oldest to Newest",
      },
      {
        text: "Date",
        text2: "Low to High",
      },
      {
        text: "Date",
        text2: "High to Low",
      },
    ],

    things: [
      {
        img: "bricks.png",
        title: "Family Apartment",
        address: "Dhanmondi, Dhaka",
        bedroom: "3 Bedrooms",
        bathroom: "2 Bathroom",
        price: "$200",
      },
      {
        img: "california.jpg",
        title: "Family Apartment",
        address: "Dhanmondi, Dhaka",
        bedroom: "3 Bedrooms",
        bathroom: "2 Bathroom",
        price: "$200",
      },
      {
        img: "house2.png",
        title: "Family Apartment",
        address: "Dhanmondi, Dhaka",
        bedroom: "3 Bedrooms",
        bathroom: "2 Bathroom",
        price: "$200",
      },
      {
        img: "mountain.jpg",
        title: "Family Apartment",
        address: "Dhanmondi, Dhaka",
        bedroom: "3 Bedrooms",
        bathroom: "2 Bathroom",
        price: "$200",
      },
      {
        img: "building.jpg",
        title: "Family Apartment",
        address: "Dhanmondi, Dhaka",
        bedroom: "3 Bedrooms",
        bathroom: "2 Bathroom",
        price: "$200",
      },
      {
        img: "about.png",
        title: "Family Apartment",
        address: "Dhanmondi, Dhaka",
        bedroom: "3 Bedrooms",
        bathroom: "2 Bathroom",
        price: "$200",
      },
      {
        img: "sea.jpg",
        title: "Family Apartment",
        address: "Dhanmondi, Dhaka",
        bedroom: "3 Bedrooms",
        bathroom: "2 Bathroom",
        price: "$200",
      },
      {
        img: "snow.png",
        title: "Family Apartment",
        address: "Dhanmondi, Dhaka",
        bedroom: "3 Bedrooms",
        bathroom: "2 Bathroom",
        price: "$200",
      },
      {
        img: "man.png",
        title: "Family Apartment",
        address: "Dhanmondi, Dhaka",
        bedroom: "3 Bedrooms",
        bathroom: "2 Bathroom",
        price: "$200",
      },
    ],
  }),
};
</script>

<style></style>
