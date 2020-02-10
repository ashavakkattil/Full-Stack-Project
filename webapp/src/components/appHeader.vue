<template>
  <div>
    <v-system-bar color="black" dark>
      <v-spacer></v-spacer>
      <h3 class="subtitle">Login/Signup</h3>
    </v-system-bar>
    <v-parallax src="https://cdn.vuetifyjs.com/images/parallax/material.jpg" height="300">
      <v-row class="align-center">
        <v-col class="text-center">
          <p class="display-4">Trails & Tales</p>
          <v-row class="justify-center">
            <v-col sm="4">
              <v-row class="justify-center">
                <v-col sm="1" class="px-0">
                  <v-icon>mdi-facebook</v-icon>
                </v-col>
                <v-col sm="1" class="px-0">
                  <v-icon>mdi-instagram</v-icon>
                </v-col>
                <v-col sm="1" class="px-0">
                  <v-icon>mdi-email</v-icon>
                </v-col>
              </v-row>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-parallax>
    <v-row class="justify-center">
      <v-app-bar class="ma-auto" dense outlined color="transparent">
        <v-container>
          <v-row class="justify-center text-center mx-auto">
            <v-col sm="1" class="px-0 homepageLink">
              <router-link to="/"><span >Home</span></router-link>
            </v-col>
            <v-col sm="1" class="px-0 homepageLink">
              <router-link to="/blog"><span >blog</span></router-link>
            </v-col>
            <v-col sm="1" class="px-0 homepageLink">
              <router-link to="/about"><span >About</span></router-link>
            </v-col>
          </v-row>
        </v-container>
      </v-app-bar>
    </v-row>
  </div>
</template>
<style scoped>
.homepageLink a{
    text-decoration: none !important;
    text-transform: uppercase;
    color: inherit;
    font-weight: bold;
    font-size: 18px
}
</style>