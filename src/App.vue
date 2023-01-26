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

    <v-main class="vmain">
      <GithubVuewer/>
    </v-main>
      <v-footer
    dark
    padless
  >
    <v-card
      flat
      tile
      class="black lighten-1 white--text text-center"
    >
      <v-card-text class="white--text pt-0">
      .  Projeto realizado para apresentação no programa Busertech da empresa de tecnologia Buser, o objetivo dessa aplicação é fixar a lógica de programação em Vue com Vuetify.  A interface pode ser pensada como a ligação entre duas aplicações devido as API consumida. Pensando num desing simples e objetivo para acessar os usuários do Github, listar seus repósitorios e suas pastas.
      </v-card-text>

      <v-divider></v-divider>

      <v-card-text class="white--text">
        {{ new Date().getFullYear() }} — <strong>Cainã Lucas</strong>
      </v-card-text>
    </v-card>
  </v-footer>

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
  display: flex;
    position: relative;
    z-index: 0;
    flex-direction: column;
    flex-wrap: wrap;
    align-content: center;
    justify-content: space-evenly
}
.vmain{
  background-color: goldenrod;
}
</style>
