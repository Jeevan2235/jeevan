<template>
  <div class="ml-16">
    <v-container>
      <v-row>
        <div v-for="link in links" :key="link">
          <v-card elevation="0" width="395px">
            <v-card class="pa-4" elevation="0" color="#f7f7f7">
              <v-card width="30em" elevation="0">
                <v-img :src="link.img" height="250"> </v-img>
                <v-card-text class="text-subtitle-1 mx-2 pa-3"
                  >{{ link.date }} {{ link.rooms }}</v-card-text
                >
                <v-card-title>{{ link.title }}</v-card-title>

                <v-divider class="mx-4 mb-2"></v-divider>

                <v-spacer></v-spacer>
                <v-icon class="ml-5 mb-2">mdi-share-variant </v-icon
                ><v-icon class="ml-5 mb-2">mdi-star-outline</v-icon>
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
        img: "california.jpg",
        title: "Finding best places to visit in California",
        date: "July 25, 2016 |",
        rooms: "Rooms & Suites",
      },
      {
        img: "building.jpg",
        title: "Finding best places to visit in California",
        date: "July 25, 2016 |",
        rooms: "Rooms & Suites",
      },
      {
        img: "car.png",
        title: "Finding best places to visit in California",
        date: "July 25, 2016 |",
        rooms: "Rooms & Suites",
      },
      // {
      //   img: "mountain.jpg",
      //   title: "Finding best places to visit in California",
      //   date: "July 25, 2016 |",
      //   rooms: "Rooms & Suites",
      // },
      // {
      //   img: "california.jpg",
      //   title: "Finding best places to visit in California",
      //   date: "July 25, 2016 |",
      //   rooms: "Rooms & Suites",
      // },
      // {
      //   img: "building.jpg",
      //   title: "Finding best places to visit in California",
      //   date: "July 25, 2016 |",
      //   rooms: "Rooms & Suites",
      // },
      // {
      //   img: "snow.png",
      //   title: "Finding best places to visit in California",
      //   date: "July 25, 2016 |",
      //   rooms: "Rooms & Suites",
      // },
      // {
      //   img: "sea.jpg",
      //   title: "Finding best places to visit in California",
      //   date: "July 25, 2016 |",
      //   rooms: "Rooms & Suites",
      // },
    ],
  }),
};
</script>

<style>
</style>