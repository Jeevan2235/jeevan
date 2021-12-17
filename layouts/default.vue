<template>
  <v-app>
    <v-app-bar height="200" color="#1c1c1c">
      <v-container>
        <v-row>
          <v-card-title>
            <v-img src="house.png" height="50" width="60" class="mr-2"></v-img>
            <h2 class="yellow--text mt-2">House Rent</h2></v-card-title
          >
          <v-spacer></v-spacer>
          <v-btn class="green--text mt-8 ml-10" elevation="0" color="#1c1c1c">
            <v-icon class="mr-2 white--text">mdi-phone</v-icon> US - 01623
            030020
          </v-btn>
          <v-btn class="green--text mt-8" elevation="0" color="#1c1c1c">
            <v-icon class="mr-2 white--text">mdi-account-box</v-icon>LOGIN /
            REGISTER
          </v-btn>
          <v-col>
            <v-btn class="mt-5 mr-13" elevation="0" color="#1c1c1c"
              ><v-icon class="ml-16 green--text">mdi-magnify</v-icon> </v-btn
            ><v-app-bar-nav-icon class="mt-4 white--text"></v-app-bar-nav-icon>
          </v-col>
        </v-row>
        <v-divider></v-divider>
        <v-row no-gutters >
          <v-btn
              v-for="link,i in links"
              :key="i"
              color="white"
              text
              rounded
              class="mx-4 mt-3"
              link
              :to="i==0?'/':'/'+link.toLowerCase()"
            >
              {{ link }}
            </v-btn>
          <v-btn class="mt-3 orange--text ml-16" color="#1c1c1c " elevation="0"
            >Booking</v-btn
          >
          <v-col class="text-center white--text" cols="12"></v-col>
        </v-row>
      </v-container>
    </v-app-bar>

    <v-main>
      <Nuxt />
    </v-main>
    
    <v-footer>
      <v-container>
        <v-row>
          <!-- cols = 12 takes whole 12 column inside row if size of device is smaller than medium devices i.e, md -->
          <!-- md = 4 takes  4 column inside row if size of device is greater or equals to medium device i.e, md -->
          <!-- this helps to make webpage content resopnsive -->
          <!-- 

            https://vuetifyjs.com/en/features/breakpoints/#breakpoint-service

            Material Design Breakpoints

            Extra small	=> xs	Small to large phone	< 600px
            Small	      => sm	Small to medium tablet	600px > < 960px
            Medium	    => md	Large tablet to laptop	960px > < 1264px*
            Large	      => lg	Desktop	1264px > < 1904px*
            Extra large	=> xl	4k and ultra-wide	> 1904px*
           
           -->
          <v-col cols="12" md="4" sm="6">
            <h2 style="color: #fca22a">About House Rent</h2>
            <v-divider class="mb-5 mt-3"></v-divider>
            <v-img src="footer-logo.png" height="50" width="245"> </v-img>
            <p class="mt-10">
              We Provide Premium Word Press, Ghost and HTML template. Our Perm
              tritium Templates is, develop gaped in a way so that the clients
              find Support. Themes are developed in a way so that the clients
              find.
            </p>
            <v-btn class="white--text" color="#fca22a" width="130" height="40"
              >More</v-btn
            >
          </v-col>

          <v-col cols="12" md="4" sm="6">
            <h2 style="color: #fca22a">Place Category</h2>
            <v-divider class="mb-8 mt-3"></v-divider>
            <p style="text-bold">
              Flat for Rent <span style="color: #fca22a">Francis</span>
            </p>
            <p>
              Flat for Rent <span style="color: #fca22a">Collins St</span>
            </p>
            <p>Flat for Rent <span style="color: #fca22a">Rose Ln</span></p>
            <p>
              Flat for Rent <span style="color: #fca22a">Cosgrave Ln</span>
            </p>
            <p>Flat for Rent <span style="color: #fca22a">Bourke St</span></p>
            <p>
              Flat for Rent <span style="color: #fca22a">Flienders Ln</span>
            </p>
          </v-col>
          <v-col cols="12" md="4" sm="6">
            <h2 style="color: #fca22a">Instagram Image</h2>
            <v-divider class="mb-8 mt-3"></v-divider>
            <v-row>
              <v-col
                v-for="n in 6"
                :key="n"
                class="d-flex child-flex"
                cols="4"
              >
                <v-img
                  :src="`https://picsum.photos/500/300?image=${n * 5 + 10}`"
                  :lazy-src="`https://picsum.photos/10/6?image`"
                  aspect-ratio="1"
                  class="grey lighten-2"
                >
                  <template v-slot:placeholder>
                    <v-row
                      class="fill-height ma-0"
                      align="center"
                      justify="center"
                    >
                      <v-progress-circular
                        indeterminate
                        color="grey lighten-5"
                      ></v-progress-circular>
                    </v-row>
                  </template>
                </v-img>
              </v-col>
            </v-row>
          </v-col>
        </v-row>
        <v-divider class="mt-16"></v-divider>
        <p class="text-center mt-8">
          Copyright ©2017 <span style="color: #fca22a">HTMLguru</span>
        </p>
      </v-container>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data(){
    return{
      links: ["Home", "Booking", "BlogSingle", "About", "Gallery", "Blog", "Contact","Account","Reservation",],
    }
  }
};
</script>

<style>
</style>