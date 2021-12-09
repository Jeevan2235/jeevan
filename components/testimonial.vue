<template>
  <div>
    <h1 class="text-center" style="font-size: 120px; font-family: Playfair Display, serif;;color: #fff">
      Testimonial
    </h1>
    <h2 class="text-center" style="font-weight: bold; font-size: 30px">
      SOME REVIEWS
    </h2>
    <div>
      <v-container>
        <v-row>
          <div v-for="link in links" :key="link">
              
            <v-card width="370px" class="mt-16 mx-3" elevation="0">
            
              <v-card class="pa-4" elevation="0">
                <v-card-title style="font-size: 1.563em; font-weight: bold">{{
                  link.title
                }}</v-card-title>
                <p class="ml-5">{{ link.text }}</p>
                <p class="ml-5">{{ link.desc }}</p>
                <v-rating class="ml-3" color="warning" value="5"></v-rating>
              </v-card>
            </v-card>
          </div>
        </v-row>
      </v-container>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    links: [
      {
        title: "Single Rakib",
        text: "Softhopper Manager",
        desc: "Amorem ipsum dolor sit amet, consectetur adipiscing elit. Cras vitae nibh nisl. Cras etitikis mauris eget lorem ultricies ferme ntum a inti diam.",
      },
      {
        title: "Single Rakib",
        text: "Softhopper Manager",
        desc: "Amorem ipsum dolor sit amet, consectetur adipiscing elit. Cras vitae nibh nisl. Cras etitikis mauris eget lorem ultricies ferme ntum a inti diam.",
      },
      {
        title: "Single Rakib",
        text: "Softhopper Manager",
        desc: "Amorem ipsum dolor sit amet, consectetur adipiscing elit. Cras vitae nibh nisl. Cras etitikis mauris eget lorem ultricies ferme ntum a inti diam.",
      },
    ],
  }),
};
</script>

<style>
</style>