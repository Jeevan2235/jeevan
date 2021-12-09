<template>
  <div>
    <v-card class="ml-2 pa-3" height="33em" width="22em" elevation="0">
      <p class="pa-2 pl-3 mt-2" style="font-weight: bold; font-size: 26px">
        Popular Posts
      </p>
      <div class="d-flex">
        <div>
          <v-container>
            <v-img src="building.jpg" height="80px" width="80px"></v-img>
          </v-container>
        </div>

        <div>
          <h4 class="pt-3" style="font-weight: 800">
            Europe’s best affordable
          </h4>
          <p>August 23, 2015</p>
        </div>
      </div>
      <v-divider class="ml-3 mr-3"></v-divider>
      <div class="d-flex">
        <div>
          <v-container>
            <v-img src="california.jpg" height="80px" width="80px"></v-img>
          </v-container>
        </div>

        <div>
          <h4 class="pt-3" style="font-weight: 800">Visiting Green Field</h4>
          <p>August 23, 2015</p>
        </div>
      </div>
      <v-divider class="ml-3 mr-3"></v-divider>
      <div class="d-flex">
        <div>
          <v-container>
            <v-img src="sea.jpg" height="80px" width="80px"></v-img>
          </v-container>
        </div>

        <div>
          <h4 class="pt-3" style="font-weight: 800">Europe’s best affordab</h4>
          <p>August 23, 2015</p>
        </div>
      </div>
      <v-divider class="ml-3 mr-3"></v-divider>
      <div class="d-flex">
        <div>
          <v-container>
            <v-img src="snow.png" height="80px" width="80px"></v-img>
          </v-container>
        </div>

        <div>
          <h4 class="pt-3" style="font-weight: 800">
            Simple Flower Arements You Can Put.
          </h4>
          <p>August 23, 2015</p>
        </div>
      </div>
    </v-card>

    <v-card class="mt-7 ml-2" elevation="0" height="25em" width="22em">
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

    <v-card class="mt-7 ml-2" elevation="0" height="22em" width="22em">
      <h2 class="pa-2 pl-6 pt-5">Ad Unit</h2>
      <v-container>
        <v-img src="best.png" class="ma-4"></v-img>
      </v-container>
    </v-card>
    <v-card class="mt-7 ml-2" elevation="0" height="22em" width="22em">
      <h2 class="pa-2 pl-6 pt-5">Tag Cloud</h2>
      <v-container >
        <v-row class=" pl-5 pt-3 " >
          <v-btn tile elevation="0" outlined style="font-size:12px;">News</v-btn>
          <v-btn tile elevation="0" outlined class="ml-2 mr-2" style="font-size:12px;">Magazine</v-btn>
          <v-btn tile elevation="0" outlined style="font-size:12px;">Lifestyle</v-btn>
        </v-row>
        <v-row class="pl-3 pt-1">
          <v-btn tile elevation="0" outlined class="ml-2 mr-2" style="font-size:12px;">Music</v-btn>
          <v-btn tile elevation="0" outlined class="ml-2 mr-2" style="font-size:12px;">Articles</v-btn>
          <v-btn tile elevation="0" outlined  class="ml-2 mr-2" style="font-size:12px;">Travels</v-btn> </v-row
        ><v-row class="pl-3 pt-1">
          <v-btn tile elevation="0" outlined  class="ml-2 mr-2" style="font-size:12px;">Sports</v-btn>
          <v-btn tile elevation="0" outlined class="ml-2 mr-2" style="font-size:12px;">Movie</v-btn>
          <v-btn tile elevation="0" outlined class="ml-2 mr-2" style="font-size:12px;">Link</v-btn>
        </v-row>
        <v-row class="pl-3 pt-1">
    <v-btn tile elevation="0" outlined class="ml-2 mr-2" style="font-size:12px;">Technology</v-btn>
          <v-btn tile elevation="0" outlined class="ml-2 mr-2" style="font-size:12px;">Fashion</v-btn>
        </v-row>
        <v-row class="pl-3 pt-1">
          <v-btn tile elevation="0" outlined class="ml-2 mr-2" style="font-size:12px;">Business</v-btn>
          <v-btn tile elevation="0" outlined class="ml-2 mr-2" style="font-size:12px;">Newspaper</v-btn>
        </v-row>
        <v-row class="pl-3 pt-1">
           <v-btn tile elevation="0" outlined class="ml-2 mr-2" style="font-size:12px;">E-book</v-btn>
          
        </v-row>
      </v-container>
    </v-card>
    
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>