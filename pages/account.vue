<template >
  <v-container>
    <v-card  width="38.8em" class="my-16 mx-auto">
      <div class="mb-4">
        <v-btn :color="login == false?'white':'success'" elevation="0" height="5em" width="22em" class="mx-0"
      @click="switchAccountVue('login')"
        >Login</v-btn
      >

      <v-btn :color="login?'white':'success'" elevation="0" height="5em" width="22em" class="mx-0"
          @click="switchAccountVue('register')"
        >Register</v-btn
      >

      </div>

      <login v-if="login"/>
      <newaccount  v-else/>
    </v-card>

  </v-container>
</template>

<script>
import newaccount from '~/components/newaccount.vue';
import Login from '~/components/login.vue';
export default {
  components: { newaccount, Login },
  data() {
    return {
      login:false,
      items: [{ icon: "mdi-view-dashboard" }],
    };
  },
  methods:{
    switchAccountVue(value){
      value == 'login'? this.login = true : this.login = false;
    }
  }
};
</script>

<style >
</style>