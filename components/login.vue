<template>
  <div>
      <v-text-field class="mx-10" outlined>
        <template v-slot:label>
          <v-icon style="vertical-align: middle"> mdi-email-outline </v-icon>
          Email
        </template>
      </v-text-field>

      <v-text-field class="mx-10" outlined>
        <template v-slot:label>
          <v-icon style="vertical-align: middle"> mdi-key-variant </v-icon>

          Password
        </template>
        <strong>
          <v-divider vertical></v-divider>
        </strong>
      </v-text-field>
      <v-card-actions>
          <v-btn
          class="mb-5 mx-auto white--text"
          width="40em"
          color="#21b55f"
          height="3.5em"
          >LogIn</v-btn
          >
      </v-card-actions>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>