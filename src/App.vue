<template>
  <v-app>
    <v-app-bar
      app
      color="gray"
      dark
    >
      <div class="d-flex align-center">
        <v-img
          alt="Asshats lo"
          class="shrink mr-2"
          contain
          src="https://images.evetech.net/Corporation/98566699_64.png"
          transition="scale-transition"
          width="40"
        />
      </div>
    </v-app-bar>

    <v-main>
      <HelloWorld/>
    </v-main>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',

  components: {
    HelloWorld,
  },

  data: () => ({
    //
  }),
};
</script>
