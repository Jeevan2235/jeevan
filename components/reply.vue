<template>
  <v-container>
    <v-card  height="33em" width="72em" elevation="0">
      <v-container>
      <h1 class="text-center ">Leave your Reply</h1>
      <v-row>
        <v-col cols="12" md="6" sd="4">
          <v-text-field label="Name*"></v-text-field>
        </v-col>
        <v-col cols="12" md="6" sd="4">
          <v-text-field label="Email*"></v-text-field>
        </v-col>
      </v-row>
      <v-col cols="12" md="12" sd="2">
        <v-text-field label="Website*"></v-text-field>
        <v-text-field label="Write a comment..."></v-text-field>
      </v-col>

      <div class="text-center">
        <v-btn rounded class="mt-3" height="2em" dark>Post a comment</v-btn>
      </div>
      </v-container>
    </v-card>

  </v-container>
</template>

<script>
export default {};
</script>

<style></style>
