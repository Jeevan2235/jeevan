<template>
  <div>
    <v-card
      v-for="thing in things"
      :key="thing"
      height="64em"
      width="21em"
      class="pt-1"
      style="background: linear-gradient(#009933 20%, #333399 90%)"
    >
      <v-card class="ml-2 mt-1 pa-3" height="63em" width="20em">
        <p class="pa-5" style="font-weight: bold; font-size: 18px">
          {{thing.title}}
        </p>
        <p><span style="color: #fba22a">{{thing.name}}</span></p>
        <v-text-field outlined label="Full Name"> </v-text-field>
        <p><span style="color: #fba22a">{{thing.number}}</span></p>
        <v-text-field outlined label="+977985542251"> </v-text-field>
        <p><span style="color: #fba22a">{{thing.email}}</span></p>
        <v-text-field outlined label="jack@gmail.com"> </v-text-field>
        <p><span style="color: #fba22a">{{thing.family}}</span></p>
        <v-text-field outlined label="1"> </v-text-field>
        <p><span style="color: #fba22a">{{thing.children}}</span></p>
        <v-text-field outlined label="1"> </v-text-field>
        <p><span style="color: #fba22a">{{thing.message}}</span></p>
        <v-text-field height="9em" outlined label="MESSAGE"> </v-text-field>
        <v-btn
          class="white--text ml-1"
          height="45"
          width="290"
          style="
            background: linear-gradient(to right, #009933 20%, #333399 90%);
          "
          >Request Booking</v-btn
        >
      </v-card>
    </v-card>
    <v-card class="mt-7" height="25em" width="22em">
      <v-img src="ad.png" height="25em"></v-img>
    </v-card>
  </div>
</template>

<script>
export default {
  data: () => ({
    things: [
      {
        title: "BOOK THIS APARTMENT",
        name: "Full Name",
        number:"Phone Number",
        email:"Emai Address",
        family:"Family Member",
        children:"Children",
        message:"Your Message",
       
      },
    ],
  }),
};
</script>

<style></style>
