<template>
  <div>
    <div style="background-color: #f7f7f7">
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
          <h3 class="mb-16">Home > <span style="color: #999999">blog</span></h3>
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
      <div class="mt-10">
        <v-container>
        <v-row>
          <v-col cols="12" md="8" sm="4">
            <blog />
          </v-col>

          <v-col cols="12" md="4" sm="4">
            <popularpost />
          </v-col>
        </v-row>
        </v-container>
      </div>

      <div>
        <v-pagination
          v-model="page"
          :length="15"
          :total-visible="7"
        ></v-pagination>
      </div>
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
