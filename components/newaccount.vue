<template >
  <div align="center">
    <v-card height="31em" width="38.8em" class="mt-16">
      <v-btn color="white" elevation="0" height="5em" width="22em" class="mx-0"
        >Sign In</v-btn
      >

      <v-btn color="white" elevation="0" height="5em" width="22em" class="mx-0"
        >New Account</v-btn
      >

      <v-text-field class="mx-10" outlined>
        <template v-slot:label>
          <v-icon style="vertical-align: middle"> mdi-account </v-icon>
          Username
        </template>
      </v-text-field>

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
      <v-checkbox class="pl-10" v-model="checkbox" label="I agree to the Terms"
        >on</v-checkbox
      >
      <v-btn
        class="mb-5 white--text"
        width="40em"
        color="#21b55f"
        height="3.5em"
        >LogIn</v-btn
      >
    </v-card>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [{ icon: "mdi-view-dashboard" }],
    };
  },
};
</script>

<style >
</style>