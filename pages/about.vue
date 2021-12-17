<template>
  <div style="background-color: #f7f7f7">
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
