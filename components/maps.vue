<template>
  <div class="mt-16" style="background-color: white">
    <h1
      class="text-center"
      style="
        font-size: 60px;
        font-family: Playfair Display, serif;
        color: #0e385d;
      "
    >
      We Are Available <br />
      For You 24/7
    </h1>
    <p class="text-center" style="font-weight: bold; color: #0e385d">
      OUR ONLINE SUPPORT SERVICE IS ALWAYS 24 HOURS
    </p>
    <v-row>
      <v-col cols="12" md="8" sm="4">
        <iframe
          class="mt-10 mb-16"
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d14130.927037028847!2d85.33106357600292!3d27.694684324752473!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x39eb199a06c2eaf9%3A0xc5670a9173e161de!2sNew%20Baneshwor%2C%20Kathmandu%2044600!5e0!3m2!1sen!2snp!4v1638266521046!5m2!1sen!2snp"
          height="350"
          style="border: 0"
          allowfullscreen=""
          loading="lazy"
        ></iframe>
      </v-col>
      <v-col cols="12" md="2" sm="6" class="mt-16">
        <v-icon color="#0e385d"> mdi-map-marker </v-icon>
        <h1 class="pt-2 ma-2" style="font-size: 22px; color: #0e385d">
          Address
        </h1>
        <p class="mt-3">
          112/B - Road 121, King/St <br />
          Melbourne Australia
        </p>
        <v-icon color="#0e385d"> mdi-phone </v-icon>
        <h1 class="pt-1 ma-2" style="font-size: 22px; color: #0e385d">Call</h1>
        <p class="mt-5">
          +99 0215469875 <br />
          666 35874692050
        </p>
      </v-col>
      <v-col cols="12" md="2" sm="6" class="mt-16">
        <v-icon color="#0e385d"> mdi-email</v-icon>
        <h1 class="pt-1 ma-2" style="font-size: 22px; color: #0e385d">Mail</h1>

        <p class="mt-5">yourmail@domain.com <br />houserent@domain.com</p>

        <v-icon color="#0e385d"> mdi-account </v-icon>
        <h1 class="pt-1 ma-2" style="font-size: 22px; color: #0e385d">
          Social account
        </h1>
        <v-btn fab dark small color="grey">
          <v-icon dark> mdi-facebook </v-icon>
        </v-btn>
        <v-btn fab dark small color="grey">
          <v-icon dark> mdi-twitter </v-icon>
        </v-btn>
        <v-btn fab dark small color="grey">
          <v-icon dark> mdi-instagram </v-icon>
        </v-btn>
        <v-btn fab dark small color="grey">
          <v-icon dark> mdi-google </v-icon>
        </v-btn>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {};
</script>

<style></style>
