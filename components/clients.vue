<template>
  <div class="mt-16">
    <div v-for="link in links" :key="link">
      <v-img src="building.jpg" height="260px" width="1600px">
        <v-container class="mt-7">
          <v-col class="d-flex">
            <h1 class="white--text mx-16" style="font-size: 60px">
              {{link.number}}
              <p style="font-size: 40px">{{link.text}}</p>
            </h1>

            <h1 class="white--text mx-10" style="font-size: 60px">
              {{link.num}}
              <p style="font-size: 40px">{{link.tex}}</p>
            </h1>

            <h1 class="white--text mx-16" style="font-size: 60px">
              {{link.num2}}
              <p style="font-size: 40px">{{link.clien}}</p>
            </h1>
            <h1 class="white--text mx-10" style="font-size: 60px">
              {{link.num3}}
              <p style="font-size: 40px">{{link.apar}}</p>
            </h1>
          </v-col>
        </v-container>
      </v-img>
    </div>
  </div>
</template>

<script>
export default {
 data: () => ({
    links: [
      {
        number:"2500",
        text:"clients",
        num:"3500",
        tex:"Booking",
        num2:"5000",
        clien:"Swimming",
        num3:"1530",
        apar:"Apartment"
      },
     
    ],

  }),
};
</script>

<style>
</style>