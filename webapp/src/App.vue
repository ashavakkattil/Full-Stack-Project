<template>
  <v-app>
    <appHeader />
    <router-view></router-view>
  </v-app>
</template>

<script>
import appHeader from "./components/appHeader";

export default {
  name: "App",

  components: {
    appHeader
  },

  data: () => ({
    //
  })
};
</script>
<style >
.container{
  max-width: 1200px
}
</style>
