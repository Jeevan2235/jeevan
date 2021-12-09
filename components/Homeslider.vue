<template>
  <div class="home">
    <v-carousel >
      <div v-for="thing in things" :key="thing">
        <v-img src="mountain.jpg" height="35em">
          <div>
            <p
              class="text-center white--text mt-16 font-weight-regular"
              style="font-size: 24px"
            >
              {{ thing.title }}
            </p>
          </div>
          <div>
            <h1
              class="text-center white--text"
              style="font-family: Playfair Display, serif; font-size: 90px"
            >
              {{ thing.heading }}
            </h1>
          </div>
          <v-container>
            <div style="padding-left: 100px; margin-right: 70px">
              <p class="text-center mt-5 white--text" style="font-size: 20px">
                {{ thing.text }}
              </p>
            </div>
          </v-container>

          <div class="text-center">
            <v-btn
              rounded
              class="white--text font-weight-bold "
              color="#fba22a"
              height="50"
              width="180"
              >Special Offer</v-btn
            >
          </div>
        </v-img>
      </div>
    </v-carousel>
  </div>
</template>

<script>
export default {
  data: () => ({
    things: [
      {
        title: "Good Service is our passion",
        heading: "Awesome apartment Villa",
        text: "No matter what the weather, no matter what the situation we are in, if we have the right perspective in life, life will always be beautiful!",
      },
    ],
  }),
};
</script>

<style>
.home {
  @media screen {
    max: width 400px;
  }
}
</style>
