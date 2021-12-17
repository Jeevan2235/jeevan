<template>
  <div>
    <v-card class=" pa-3" height="33em" width="22em" elevation="0">
      <p class="pa-2 pl-3 mt-2" style="font-weight: bold; font-size: 26px">
        Popular Posts
      </p>

      <v-container>
        <v-row>
          <v-col cols="12" md="4" sd="6">
            <v-img src="building.jpg" height="80px" width="80px"></v-img
          ></v-col>
          <v-col>
            <h4 class="pt-3" style="font-weight: 800">
              Europe’s best affordable
            </h4>
            <p>August 23, 2015</p>
          </v-col>
        </v-row>
      </v-container>

      <v-divider class=" mr-3"></v-divider>

      <v-container>
        <v-row>
          <v-col cols="12" md="4" sd="6">
            <v-img src="california.jpg" height="80px" width="80px"></v-img>
          </v-col>
          <v-col>
            <h4 class="pt-3" style="font-weight: 800">Visiting Green Field</h4>
            <p>August 23, 2015</p>
          </v-col>
        </v-row>
      </v-container>

      <v-divider class=" mr-3"></v-divider>

      <v-container>
        <v-row>
          <v-col cols="12" md="4" sd="6">
            <v-img src="sea.jpg" height="80px" width="80px"></v-img>
          </v-col>
          <v-col>
            <h4 class="pt-3" style="font-weight: 800">
              Europe’s best affordab
            </h4>
            <p>August 23, 2015</p>
          </v-col>
        </v-row>
      </v-container>

      <v-divider class=" mr-3"></v-divider>

      <v-container>
        <v-row>
          <v-col cols="12" md="4" sd="6">
            <v-img src="snow.png" height="80px" width="80px"></v-img>
          </v-col>
          <v-col>
            <h4 class="pt-3" style="font-weight: 800">
              Simple Flower Arements You Can Put.
            </h4>
            <p>August 23, 2015</p>
          </v-col>
        </v-row>
      </v-container>
    </v-card>

    <v-card class="mt-7 " elevation="0" height="25em" width="22em">
      <h2 class="pa-5">Categories</h2>
      <v-container class="pa-5">
        <v-container>
          <v-row class="pl-3 pr-3" style="font-weight: bold">
            <p>Travels</p>
            <v-spacer></v-spacer>
            <p>45</p>
          </v-row>
          <v-divider></v-divider>
        </v-container>
        <v-container>
          <v-row class="pl-3 pr-3" style="font-weight: bold">
            <p>Lifestyle</p>
            <v-spacer></v-spacer>
            <p>55</p>
          </v-row>
          <v-divider></v-divider>
        </v-container>
        <v-container>
          <v-row class="pl-3 pr-3" style="font-weight: bold">
            <p>Fashion</p>
            <v-spacer></v-spacer>
            <p>20</p>
          </v-row>
          <v-divider></v-divider>
        </v-container>
        <v-container>
          <v-row class="pl-3 pr-3" style="font-weight: bold">
            <p>Music</p>
            <v-spacer></v-spacer>
            <p>30</p>
          </v-row>
          <v-divider></v-divider>
        </v-container>
        <v-container>
          <v-row class="pl-3 pr-3" style="font-weight: bold">
            <p>Video</p>
            <v-spacer></v-spacer>
            <p>50</p>
          </v-row>
          <v-divider></v-divider>
        </v-container>
      </v-container>
    </v-card>

    <v-card class="mt-7 " elevation="0" height="22em" width="22em">
      <h2 class="pa-2 pl-6 pt-5">Ad Unit</h2>
      <v-container>
        <v-img src="best.png" class="ma-4"></v-img>
      </v-container>
    </v-card>
    <v-card class="mt-7 " elevation="0" height="23em" width="22em">
      <h2 class="pa-2 pl-6 pt-5">Tag Cloud</h2>
      <v-container  >
        <v-row class="pl-5 pt-3" v-for="link in links"
          :key="link">
          <v-btn tile elevation="0" outlined style="font-size: 12px"
            >{{link}}</v-btn
          >
          
        </v-row>
      </v-container>
    </v-card>
  </div>
</template>

<script>
export default {
  data: () => ({
    links: ["News","Magazine", "Lifestyle","News","Magazine", "Lifestyle"
    ]
  })
};
</script>

<style></style>
