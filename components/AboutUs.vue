<template>
  <div class="mt-10" style="background-color: #ffffff">
    <v-container>
      <h1
        class="text-center mt-16"
        style="
          font-size: 60px;
          font-family: Playfair Display, serif;
          color: #0e385d;
        "
      >
        About Us
      </h1>
      <h3 class="text-center" style="color: #0e385d">
        WELCOME TO OUR HOUSE RENT COMPANY
      </h3>
      <v-row class="mt-10">
        <v-col cols="1">
          <p class="font-weight-bold my-16 ml-10">About <br />Company</p>
          <p class="font-weight-bold my-16 ml-10">Terms& <br />Conditions</p>
          <p class="font-weight-bold my-16 ml-10">Our <br />speciality</p>
          <p class="font-weight-bold my-16 ml-10">
            Our <br />
            speciality
          </p>
        </v-col>

        <v-col>
          <div>
            <v-timeline align-top dense>
              <v-timeline-item color="orange" small>
                <div v-for="thing in things" :key="thing">
                  <v-row>
                    <v-col>
                      <p>
                        {{ thing.text }}
                      </p>
                      <p v-for="link in links" :key="link">
                        {{ link }}
                      </p>
                    </v-col>
                    <v-col>
                      <v-img :src="thing.img" height="350px" width="450px">
                      </v-img>
                    </v-col>
                  </v-row>
                </div>
              </v-timeline-item>
            </v-timeline>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  data: () => ({
    links: [
      "• Amorem ipsum dolor sit amet, consectetur",
      "• Cras etitikis mauris egeth lorem ultricies",
      "• Amorem ipsum dolor sit amet, consectetur",
      "• Cras etitikis mauris egeth lorem ultricies",
      "• Amorem ipsum dolor sit amet, consectetur",
      "• Cras etitikis mauris egeth lorem ultricies",
      "• Amorem ipsum dolor sit amet, consectetur",
    ],
    things: [
      {
        text: "Amorem ipsum dolor sit amet, consectetur adipiscing elit. Cras vitae nibh nisl. Cras etitikis mauris egeth lorem ultricies ferme is ntum a inti diam. Morbi mollis pellden tesque offs aiug ueia nec rhoncus. Nam ute ultricies. Cras etitikis mauris eget lorem ultricies ferme ntum a inti diam. Morbi mollis pellen tesque offs aiug ueia nec rhoncus. Nam ute ultricies.",
        img: "about.png",
      },
    ],
  }),
};
</script>

<style>
</style>