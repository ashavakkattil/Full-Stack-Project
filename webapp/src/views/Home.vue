<template>
  <v-container class="ma-auto">
    <template v-if="$vuetify.breakpoint.mdAndUp">
      <v-row>
        <v-col cols="8">
          <v-card height="500">
            <v-img
              src="https://www.designlabthemes.com/preview/type/files/2017/07/red-792139_1920-800x500.jpg"
              height="inherit"
            />
          </v-card>
        </v-col>
        <v-col cols="4">
          <v-card height="240" class="mb-6">
            <v-img
              src="https://www.designlabthemes.com/preview/type/files/2017/07/cake-1839134_1920-800x500.jpg"
              height="inherit"
            ></v-img>
          </v-card>

          <v-card height="240">
            <v-img
              src="https://www.designlabthemes.com/preview/type/files/2017/07/mobile-791164-800x500.jpg"
              height="inherit"
            ></v-img>
          </v-card>
        </v-col>
      </v-row>
    </template>
    <template v-else-if="$vuetify.breakpoint.smOnly">
      <v-row>
        <v-col>
          <v-row>
            <v-col cols="12">1pic</v-col>
          </v-row>
          <v-row>
            <v-col cols="6">2pics</v-col>
            <v-col cols="6">2pics</v-col>
          </v-row>
        </v-col>
      </v-row>
    </template>
    <template v-else>
      <v-row>
        <v-col cols="12">2pics</v-col>
        <v-col cols="12">2pics</v-col>
        <v-col cols="12">2pics</v-col>
      </v-row>
    </template>
    <v-row v-if="$vuetify.breakpoint.mdAndUp">
      <v-col cols="8"><blogList/></v-col>
      <v-col cols="4">
        <sideBar />
      </v-col>
    </v-row>
    <v-row v-else>
      <v-col cols="12"><blogList/></v-col>
      <v-col cols="12">
        <sideBar />
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import sideBar from "../components/sideBar";
import blogList from "../components/blogListView";
export default {
  name: "home",
  components: { sideBar, blogList },
  data() {
    return {
      items: [
        {
          src:
            "https://www.designlabthemes.com/preview/type/files/2017/07/red-792139_1920-800x500.jpg"
        },
        {
          src:
            "https://www.designlabthemes.com/preview/type/files/2017/07/cake-1839134_1920-800x500.jpg"
        },
        {
          src:
            "https://www.designlabthemes.com/preview/type/files/2017/07/mobile-791164-800x500.jpg"
        }
      ]
    };
  }
};
</script>
<style scoped>
</style>
