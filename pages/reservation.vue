<template>
  <div style="background-color: #f7f7f7">
    <div>
      <div
        class="text-center"
        style="
          background: linear-gradient(to right, #009933 20%, #333399 90%);
          height: 15em;
        "
      >
        <h1 class="pt-15 white--text" style="font-size: 45px">House</h1>
        <p style="font-weight: bold; font-size: 20px">
          More Details About Apartment
        </p>
      </div>
      <v-container>
        <p style="font-weight: bold">Home > Apartment Single Page</p>
      </v-container>

      <v-container>
        <v-row>
          <v-col cols="12" md="8" sm="4">
            <photo />
            <pricedetails />
            <propertydetails />
            <apartmentoverview />
          </v-col>
          <v-col cols="12" md="4" sm="4">
            <bookingpage />
          </v-col>
        </v-row>
      </v-container>

      <div>
        <v-container class="pl-8 mt-16"> </v-container>
        <related />
        <div style="background-color: #f7f7f7">
          <contactus />
        </div>

        <maps />
      </div>
    </div>
  </div>
</template>

<script>
import Apartmentoverview from "~/components/apartmentoverview.vue";
import bookingpage from "~/components/bookingpage.vue";
import Contactus from "~/components/contactus.vue";
import Footer from "~/components/footer.vue";
import Maps from "~/components/maps.vue";
import Propertdetails from "~/components/pricedetails.vue";
import Related from "~/components/related.vue";

export default {
  components: {
    bookingpage,
    Propertdetails,
    Apartmentoverview,
    Related,
    Contactus,
    Maps,
    Footer,
  },
  data: () => ({
    links: ["Home", "Booking", "House", "Pages", "About", "Blog", "Contact"],
  }),
};
</script>

<style></style>
