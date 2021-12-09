<template>
  <div>
    <v-container >
      <v-card class="ml-9 pa-16" height="33em" width="72em" elevation="0">
        <h1 class="text-center pa-10">Leave your Reply</h1>
        <v-row>
          <v-col>
            <v-text-field label="Name*"></v-text-field>
          </v-col>
          <v-col>
            <v-text-field label="Email*"></v-text-field>
          </v-col>
        </v-row>
        <v-text-field label="Website*"></v-text-field>
        <v-text-field label="Write a comment..."></v-text-field>
        <div class="text-center">
        <v-btn rounded
                class="mt-3"
                height="2em"
                dark>Post a comment</v-btn>
                </div>
      </v-card>
    </v-container>
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>