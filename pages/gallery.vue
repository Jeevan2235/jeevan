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
        <h1 class="pt-15 white--text" style="font-size: 45px">Gallery</h1>
        <p style="font-weight: bold; font-size: 20px">All gallery and video</p>
      </div>
    </div>

    <div style="background-color: #f7f7f7">
      <v-container>
        <h3 class="mb-16 ml-16">Home > Gallery</h3>

        <h1 class="text-center" style="font-size: 60px">PHOTO GALLERY</h1>

        <v-row>
          <v-col v-for="n in 12" :key="n" class="d-flex child-flex" cols="3">
            <v-img
              :src="`https://picsum.photos/500/300?image=${n * 5 + 15}`"
              :lazy-src="`https://picsum.photos/10/6?image=${n * 5 + 15}`"
              aspect-ratio="1"
              class="grey lighten-2"
            >
              <template v-slot:placeholder>
                <v-row class="fill-height ma-0" align="center" justify="center">
                  <v-progress-circular
                    indeterminate
                    color="grey lighten-5"
                  ></v-progress-circular>
                </v-row>
              </template>
            </v-img>
          </v-col>
        </v-row>
        <div class="text-center">
          <v-btn
            color="#0e385d"
            class="white--text mt-8"
            height="40"
            width="200"
            >Load More</v-btn
          >
        </div>

        <h1 class="text-center mt-16 mb-5" style="font-size: 60px">VIDEO GALLERY</h1>
        <v-row>
          <v-col v-for="n in 12" :key="n" class="d-flex child-flex" cols="3">
            <v-img
              :src="`https://picsum.photos/500/300?image=${n * 5 + 15}`"
              :lazy-src="`https://picsum.photos/10/6?image=${n * 5 + 15}`"
              aspect-ratio="1"
              class="grey lighten-2"
            >
              <template v-slot:placeholder>
                <v-row class="fill-height ma-0" align="center" justify="center">
                  <v-progress-circular
                    indeterminate
                    color="grey lighten-5"
                  ></v-progress-circular>
                </v-row>
              </template>
            </v-img>
          </v-col>
        </v-row>
        <div class="text-center">
          <v-btn
            color="#0e385d"
            class="white--text mt-8"
            height="40"
            width="200"
            >Load More</v-btn
          >
        </div>
      </v-container>
    </div>
   
  </div>
</template>

<script>
export default {
  data: () => ({
    links: ["Home", "Booking", "House", "Pages", "About", "Blog", "Contact"],
  }),
};
</script>

<style>
</style>