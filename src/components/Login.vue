<template>
    <div id="app">
  <v-app id="inspire">
    <v-content>
      <v-container fluid fill-height>
        <v-layout align-center justify-center>
          <v-flex xs12 sm8 md4>
            <v-card class="elevation-12">
              <v-toolbar dark color="cyan darken-4">
                <div class="cen">
                <v-toolbar-title>Login Here</v-toolbar-title>
                </div>
                <v-spacer></v-spacer>
                <v-tooltip bottom>
                  

                </v-tooltip>
              </v-toolbar>
              <v-card-text>
                <v-form>
                  <v-text-field prepend-icon="phone" name="phone" label="Phone Number" type="text"></v-text-field>                
                  <v-text-field prepend-icon="lock" name="password" label="Password" id="password" type="password"></v-text-field>
                  <v-text-field prepend-icon="group" name="group" label="Group Name" type="text"></v-text-field>
                  <v-text-field prepend-icon="lock" name="group password" label="Group Password" type="password"></v-text-field>
                </v-form>
              </v-card-text>
              <v-card-actions>
                <v-spacer></v-spacer>
                <v-btn dark color="cyan darken-4">Login</v-btn>
                <div class="me">
                <router-link to = "/register">
                <v-btn dark color="cyan darken-4">Register</v-btn>      
                </router-link>
                </div>
              </v-card-actions>
            </v-card>
          </v-flex>
        </v-layout>
      </v-container>
    </v-content>
  </v-app>
</div>
</template>

<script>
  export default {
    data: () => ({
      drawer: null
    }),
    props: {
      source: String
    }
  }
</script>

<style>
.cen{
  text-align: center
}
.me{
  margin-left: 10px;
  text-decoration: none;
}
div a{
  text-decoration: none;
}
</style>
