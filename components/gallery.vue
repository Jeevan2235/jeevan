<template>
  <div class="mt-16 d-flex" style="background-color: #ffffff">
    <div v-for="thing in things" :key="thing" style="flex: 30%">
      <v-col class="pa-0">
        <v-card elevation="0" width="300px" class="mt-5 ml-7">
          <v-card elevation="0" >
            <v-img :src="thing.img" height="18em"> </v-img>

            <div v-for="link in links" :key="link">
              <v-img class="mt-3" :src="link.img" height="18em"> </v-img>
            </div>
          </v-card>
        </v-card>
      </v-col>

      <v-card elevation="0" width="300px" class="mt-5 ml-7"> </v-card>
    </div>
    <div class="mt-10 ml-10" style="flex: 50%">
      <h1  style="font-size: 70px; font-family:Playfair Display, serif; color: #0e385d">Our <br />Photo <br />Gallery</h1>
      <p style=" font-weight:bold; font-size: 25px; color:#66666f">Best of our <br />Event portfolio Photos</p>
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
    </div>
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

    links: [
      {
        img: "house2.png",
      },
    ],
  }),
};
</script>

<style></style>
