<template>
  <div style="background-color: #f7f7f7">
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
      <h1 class="text-center" style="font-size: 60px; color: #0e385d">
        Map & Directions
      </h1>
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

      <h1 class="text-center mt-8" style="font-size: 60px; color: #0e385d">
        Contact us <br />live
      </h1>

      <div class="mt-15">
        <v-row>
          <v-col cols="12" md="4" sm="4">
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
          </v-col>
          <v-col cols="12" md="8" sm="4">
            <h1 class="text-center" style="font-size: 24px">Have a question</h1>
            <v-card
              class="mt-10"
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
                    color="#0e385d"
                    >Submit</v-btn
                  >
                </div>
              </v-container>
            </v-card>
          </v-col>
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

<style></style>
