<template>
  <div style="background-color: #f7f7f7">
    <homeslider />
    <weprovide />
    <rates />
    <about-us />
    <rooms />
    <clients />\
    <gallery />
    <contactus />
    <testimonial />
    <maps />
      <h1 class=" mt-16 text-center" style="color: #0e385d; font-size: 60px;font-family: Playfair Display, serif;">Our Blog Post</h1>
      <h4 class="text-center" style="color: #0e385d;">OUR NEWS FEED</h4>
    <div>
      <v-container>
    <blog />
    </v-container>
    <div class="text-center">
        <v-btn
          
          color="#fca22a"
          elevation="0"
          class="white--text mt-5 mb-16"
          height="45"
          width="180"
          >Show All</v-btn
        >
      </div>
    </div>
    <div>
    </div>

  </div>
</template>

<script>
import AboutUs from "~/components/AboutUs.vue";
import Blog from "~/components/blog.vue";
import Clients from "~/components/clients.vue";
import Contactus from "~/components/contactus.vue";
import Footer from '~/components/footer.vue';
import Gallery from "~/components/gallery.vue";
import Homeslider from "~/components/Homeslider.vue";
import Maps from "~/components/maps.vue";
import Rooms from "~/components/rooms.vue";
import Testimonial from "~/components/testimonial.vue";
import Weprovide from "~/components/weprovide.vue";

import Rates from "./rates.vue";

export default {
  components: {
    Homeslider,
    Weprovide,
    AboutUs,
    Rates,
    Rooms,
    Clients,
    Gallery,
    Contactus,
    Testimonial,
    Maps,
    Blog,
    Footer,
  },
  data: () => ({
    links: ["Home", "Booking", "House", "Pages", "About", "Blog", "Contact"],
  }),
};
</script>

<style>
</style>