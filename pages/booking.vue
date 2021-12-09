<template>
  <div>
    <div style="background-color: #f7f7f7">
      <v-app-bar height="135px" color="#1c1c1c">
        <v-container>
          <v-row>
            <v-card-title>
              <v-img
                src="house.png"
                height="50"
                width="60"
                class="mr-2"
              ></v-img>
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
              ><v-app-bar-nav-icon
                class="mt-4 white--text"
              ></v-app-bar-nav-icon>
            </v-col>
          </v-row>
          <v-divider></v-divider>
          <v-row no-gutters>
            <v-btn
              v-for="link in links"
              :key="link"
              color="white"
              text
              rounded
              class="mx-4 mt-3"
            >
              {{ link }}
            </v-btn>
            <v-btn
              class="mt-3 orange--text ml-16"
              color="#1c1c1c "
              elevation="0"
              >Booking</v-btn
            >
            <v-col class="text-center white--text" cols="12"></v-col>
          </v-row>
        </v-container>
      </v-app-bar>
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
        <h3 class="mb-16 ml-16">
          Home > <span style="color: #999999">Apartment List For Booking</span>
        </h3>
        <v-row>
          <v-card
            class="d-flex justify-start mb-6 pl-16 mt-8"
            flat
            tile
            color="#f7f7f7"
          >
            <v-card
              v-for="popular in popular"
              :key="popular"
              color="#e8e8e8"
              elevation="0"
              height="4.5em"
              width="9em"
              class="ml-2 text-center"
            >
              <h3 class="mt-3">{{ popular.text }}</h3>
              <v-card-text style="margin-top:-20px">{{ popular.text2 }}</v-card-text>
            </v-card>
          </v-card>
          <v-spacer></v-spacer>

          <v-select 
            solo
            class="ml-10 pr-7 mt-8"
            height="4em"
            :items="items"
            label="Category"
          >
          </v-select>
        </v-row>
        <div class="ml-16">
          <v-container>
            <v-row>
              <div v-for="thing in things" :key="thing">
                <v-card elevation="0" width="365px" class="mt-5">
                  <v-card class="pa-2" elevation="0" color="#f7f7f7">
                    <v-card elevation="0" outlined>
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
                  </v-card>
                </v-card>
              </div>
            </v-row>

            <div class="text-center">
              <v-btn
                class="white--text mt-15"
                color= "#0e385d"
                height="45"
                width="150"
                >Load More</v-btn
              >
            </div>
          </v-container>
        </div>
      </v-container>
    </div>
    <v-footer>
        <v-container>
          <v-row>
            <v-col>
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

            <v-col>
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
            <v-col>
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
      },{

      text:"Date",
      text2:"High to Low",
      }
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
