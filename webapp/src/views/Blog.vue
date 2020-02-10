<template>
  <v-container>
    <v-row v-if="$vuetify.breakpoint.mdAndUp">
      <v-col cols="8">All blogs</v-col>
      <v-col cols="4">
        <sideBar />
      </v-col>
    </v-row>
    <v-row v-else>
      <v-col cols="12">All blogs</v-col>
      <v-col cols="12">
        <sideBar />
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import sideBar from "../components/sideBar";

export default {
  name: "Blog",
  components: {
    sideBar
  }
};
</script>
