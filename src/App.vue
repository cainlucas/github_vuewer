<template>
  <v-app>
    <v-app-bar class="vbar"
      app
      color="black"
      dark
    >
      <div class="d-flex align-center">
        <v-img
          src="https://logosmarcas.net/wp-content/uploads/2020/12/GitHub-Simbolo.png"
          transition="scale-transition"
          width="180"
        />

        <!-- <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
        /> -->
      </div>

      <v-spacer></v-spacer>

      <!-- <v-btn
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
        text
      > -->
      <!-- </v-btn> -->
    </v-app-bar>

    <v-main>
      <GithubVuewer/>
    </v-main>
  </v-app>
</template>

<script>
import GithubVuewer from './components/GithubVuewer';

export default {
  name: 'App',

  components: {
    GithubVuewer,
  },

  data: () => ({
    //
  }),
};
</script>
<style>
.vbar{
  background-color: black;
  display: flex;
    position: relative;
    z-index: 0;
    flex-direction: column;
    flex-wrap: wrap;
    align-content: center;
    justify-content: space-evenly
}
</style>
