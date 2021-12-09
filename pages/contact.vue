<template>
  <div style="background-color: #f7f7f7">
    <v-app-bar height="135px" color="#1c1c1c">
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
              v-for="link in links"
              :key="link"
              color="white"
              text
              rounded
              class="mx-4 mt-3"
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
  
    <div
      class="text-center"
      style="
        background: linear-gradient(to right, #009933 20%, #333399 90%);
        height: 15em;
      "
    >
      <h1 class="pt-15 white--text" style="font-size: 45px">Contact</h1>
      <p style="font-weight: bold; font-size: 20px">Contact with us</p>
    </div>
    <v-container>
      <p>Home > Contact</p>
      <p class="mt-5 text-center" style="font-size: 24px">Find Our location</p>
      <h1 class="text-center" style="font-size: 60px; color: #0e385d">Map & Directions</h1>
      <p class="text-center" style="font-weight: bold; font-size: 20px">
        Find out how to find us from your current location
      </p>

      <iframe
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3532.2227088972427!2d85.33026571483933!3d27.710409231964743!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x39eb190b6cfae8cd%3A0xb54327d56a797ef6!2sGyaneshwor%2C%20Kathmandu%2044600!5e0!3m2!1sen!2snp!4v1638250946704!5m2!1sen!2snp"
        width="1100"
        height="550"
        class="ml-5"
        style="border: 0"
        allowfullscreen=""
        loading="lazy"
      ></iframe>

      <h1 class="text-center mt-8" style="font-size: 60px;color: #0e385d">
        Contact us <br />live
      </h1>

      <div class="d-flex">
        <div class="mt-15">
          <v-row>
            <v-icon style="color: #0e385d"> mdi-map-marker </v-icon>
            <h1 class="pt-2 ma-2" style="font-size: 22px; color: #0e385d">
              Address
            </h1>
          </v-row>

          <p class="mt-3">
            112/B - Road 121, King/St <br />
            Melbourne Australia
          </p>

          <v-row class="mt-8">
            <v-icon style="color: #0e385d"> mdi-email</v-icon>
            <h1 class="pt-1 ma-2" style="font-size: 22px; color: #0e385d">
              Mail
            </h1>
          </v-row>
          <p class="mt-5">yourmail@domain.com <br />houserent@domain.com</p>

          <v-row class="mt-8">
            <v-icon style="color: #0e385d"> mdi-phone </v-icon>
            <h1 class="pt-1 ma-2" style="font-size: 22px; color: #0e385d">
              Call
            </h1>
          </v-row>
          <p class="mt-5">
            +99 0215469875 <br />
            666 35874692050
          </p>

          <v-row class="mt-8">
            <v-icon> mdi-account </v-icon>
            <h1 class="pt-1 ma-2" style="font-size: 22px; color: #0e385d">
              Social account
            </h1>
          </v-row>
          <div class="mt-3">
            <v-btn class="mx-2" fab dark small color="grey">
              <v-icon dark> mdi-facebook </v-icon>
            </v-btn>
            <v-btn class="mx-2" fab dark small color="grey">
              <v-icon dark> mdi-twitter </v-icon>
            </v-btn>
            <v-btn class="mx-2" fab dark small color="grey">
              <v-icon dark> mdi-instagram </v-icon>
            </v-btn>
            <v-btn class="mx-2" fab dark small color="grey">
              <v-icon dark> mdi-google </v-icon>
            </v-btn>
          </div>
        </div>

        <div class="mt-15 pl-16 ml-16">
          <h1 class="text-center" style="font-size: 24px">Have a question</h1>
          <v-card
            class="ml-16 mt-10"
            height="33em"
            width="45em"
            elevation="0"
            outlined
            style="background-color: #fafafa"
          >
            <h1 class="pt-8 text-center pr-12" style="font-size: 24px">
              Send Us A email
            </h1>

            <v-container class="pa-16">
              <v-row>
                <v-col>
                  <v-text-field label="Name*"></v-text-field>
                </v-col>
                <v-col>
                  <v-text-field label="Email*"></v-text-field>
                </v-col>
              </v-row>
              <v-text-field label="Website*"></v-text-field>
              <v-text-field
                outlined
                label="Your Message*"
                height="10em"
              ></v-text-field>
              <div class="text-center">
                <v-btn
                  class="white--text"
                  height="50"
                  width="180"
                  color= "#0e385d"
                  
                  >Submit</v-btn
                >
              </div>
            </v-container>
          </v-card>
        </div>
      </div>
    </v-container>
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
  }),
};
</script>

<style></style>
