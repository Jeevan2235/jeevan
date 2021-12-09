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
        <h1 class="pt-15 white--text" style="font-size: 45px">Blog</h1>
        <p style="font-weight: bold; font-size: 20px">Our all News feed</p>
      </div>
    </div>

    <div style="background-color: #f7f7f7">
      <div>
        <v-container>
          <h3 class="mb-16 ml-16">
            Home > <span style="color: #999999">blog</span>
          </h3>
          <v-row>
            <h3 v-for="thing in things" :key="thing">
              <v-btn
                elevation="0"
                height="3.5em"
                class="ml-16"
                style="background-color: #ffffff"
                width="11em"
              >
                {{ thing }}
              </v-btn>
            </h3>
          </v-row>
        </v-container>
      </div>

      <div style="float: right">
        <v-container class="mr-16 pr-16">
          <popularpost />
        </v-container>
      </div>
      <div>
        <blog />
      </div>
      <div>
        <v-pagination
          v-model="page"
          :length="15"
          :total-visible="7"
        ></v-pagination>
      </div>
    </div>
    <div>
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
  </div>
</template>

<script>
import blog from "~/components/blog.vue";
import Popularpost from "~/components/popularpost.vue";
export default {
  components: { blog, Popularpost },
  data: () => ({
    links: ["Home", "Booking", "House", "Pages", "About", "Blog", "Contact"],
    return: {
      page: 1,
    },
    things: ["Recent / News", "Popular", "Trending"],
  }),
};
</script>

<style></style>
