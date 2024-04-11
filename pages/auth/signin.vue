<template>
  <v-row align-self="center" justify="center">
    <v-col cols="12" sm="8" md="4" align-self="center">
      <v-card class="elevation-4 text-left" >
        <v-card-title class="fancy-title align-center justify-center">Trello</v-card-title><v-card-text>
          <v-form>
            <v-text-field
              label="Login"
              name="login"
              prepend-icon="mdi-account"
              type="text"
              v-model="auth.email"
            ></v-text-field>

            <v-text-field
              label="Password"
              name="password"
              prepend-icon="mdi-lock"
              type="password"
              v-model="auth.password"
            ></v-text-field>
          </v-form>
        </v-card-text>
        <v-card-actions class="text-center">
          <v-btn
            class="login-button"
            @click=""
            depressed
            large
            >Login</v-btn
          >
        </v-card-actions>
      </v-card>

    </v-col>
  </v-row>
</template>

<script>
export default {
  name: "SignInPage",
  data(){
    return {
      auth: {
        email: '',
        password: ''
      }

    }
  }
}
</script>

<style>

</style>
