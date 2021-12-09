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
        height: 13em;
      "
    >
      <h1 class="pt-15 white--text" style="font-size: 45px">About</h1>
      <p style="font-weight: bold; font-size: 20px">About our company</p>
    </div>
    <v-container>
      <h3 class="ml-16">Home > About</h3>

     <div style="color:#0b5a8d">
       <h1 class="text-center mt-10 pl-16 " style="  font-size: 45px;">
          Why <br />Choose Us
        </h1>
        <p class="text-center pl-16 ">Best offers from the house chef</p>
     </div>
      <div style="padding-right: 50px">
        
        <v-row>
          <v-col>
            <h1 class="ml-16" style="font-size: 65px; color:#06736d">
              Best <br />
              Rent Service, <br />
              enjoy your <br />life
            </h1>
          </v-col>

          <v-col class="mr-16">
            <p class="mt-10" style="font-size: 18px">
              Sed pellentesque pulvinar arcu ac congue. Sed sed est nec justo
              maximus blandit. Curabitur lacinia, eros sit amet maximus
              suscipit, magna sapien veneuynatis eros, et gravida urna massa ut
              lectus. Quisque lacinia laciunia viverra. Nullram nec est et lorem
              sodales ornare a in sapien. In trtset urna marximus, conse ctetur
              iligula in, gravida erat. Nullam digniifssrim hendrerit auctor.
              Sed varius, dolor vitae iaculis condim rtweentum, massa nisl
              cursus sapien, gravida ultrices nisi dolor non erat.
            </p>
          </v-col>
        </v-row>
      </div>
      <div>
        <div class="text-center">
          <v-avatar size="130" class="ml-16">
            <v-img color="primary" src="men.png" class="text-center"></v-img>
          </v-avatar>
        </div>
        <h1 class="text-center mt-16" style="font-size: 36px; color:#0b5a8d">
          Dr. Abdus Sabbir
        </h1>
        <p class="text-center">Rent House Admin</p>
        <v-container>
          <p class="text-center">
            Cras et mauris eget lorem ultricies fermentum a in diam. Morbi
            mollis pesllentesque aug ue nec rhoncus.
            <br />
            Nam ut ogrci augue. Phasellus ac venenatis orci. Nulalam iaculis lao
            reet maa, vitae tempus ante <br />tincidunte et. dolor st ametisnj,
            consectetur adipiscing elit. Cras vitaie nbh nisl. Cras et mauis
            eget
            <br />
            loremams ultricies ferme ntum a in diam.Nam ut orci augue. Pha
            sellus ac venen adatis orci. Nullam <br />iaculis lao reetings maa,
            vitae tempus ante tincidunte et.
          </p>
        </v-container>
        <v-row class="pl-16">
          <p class="ml-16 mt-16" style="font-weight:bold">
            Follow me: <v-icon class="pa-2"  style="color:#0b5a8d">mdi-google-play</v-icon
            ><v-icon class="pa-2" style="color:#0b5a8d">mdi-facebook</v-icon
            ><v-icon class="pa-2" style="color:#0b5a8d">mdi-youtube</v-icon
            ><v-icon class="pa-2" style="color:#0b5a8d">mdi-twitter</v-icon
            ><v-icon class="pa-2" style="color:#0b5a8d">mdi-gmail</v-icon
            ><v-icon class="pa-2" style="color:#0b5a8d">mdi-yahoo</v-icon>
          </p>
          <v-spacer></v-spacer>
          <p class="pr-16 mt-16">John</p>
        </v-row>
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

<style>




</style>
