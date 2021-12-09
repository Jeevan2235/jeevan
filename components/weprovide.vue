<template>
  <div>
    <v-row>
      <v-card tile style="margin-top: -28px" height="2.5em" width="10em">
        <p class="pl-8 pa-2" style="font-size: 18px; font-weight: bold">
          We Provide
        </p>
      </v-card>

      <v-spacer></v-spacer>

      <v-btn tile style="margin-top: -45px" height="4em" width="9em"> </v-btn>
    </v-row>
    <v-row>
      <v-card
        v-for="link in links"
        :key="link"
       elevation="0"
       outlined
       tile

      >
        <v-card color="#f7f7f7" class="pt-8 pl-5" outlined height="8em" width="7.9em">
          <v-icon class="pl-8 " 
            >{{ link.icon }}
          </v-icon>
          <p class="text-center pt-3" style="font-weight:bold;">{{link.text}}</p>
        </v-card>
      </v-card>
    </v-row>
  </div>
</template>

<script>
export default {
  data: () => ({
    links: [
      {
        icon: "mdi-warehouse",
        text: "Family House",
      },
      {
        icon: "mdi-facebook",
        text: "Apartment",
      },
      {
        icon: "mdi-account-tie",
        text: "Sublet",
      },
      {
        icon: "mdi-car-key",
        text: "Bachelor",
      },
      {
        icon: "mdi-warehouse",
        text: "Office",
      },
      {
        icon: "mdi-facebook",
        text: "Garage",
      },
      {
        icon: "mdi-warehouse",
        text: "Factory",
      },
      {
        icon: "mdi-home-floor-a",
        text: "Hall Room",
      },
      {
        icon: "mdi-warehouse",
        text: "Warehouse",
      },
      {
        icon: "mdi-facebook",
        text: "Female Mess",
      },
      {
        icon: "mdi-warehouse",
        text: "Garage",
      },
      {
        icon: "mdi-home-floor-a",
        text: "Office",
      },
    ],
  }),
};
</script>

<style></style>
