<template>
  <v-container>
    <v-row class="text-center">
      <v-col cols="12">
        <v-img
          :src="require('../assets/logo.svg')"
          class="my-5"
          transition="scale-transition"
          contain
          height="300"
        />
      </v-col>
      <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-5">
          Welcome to Asshats in DerpSpace
        </h1>
        <p class="subheading font-weight-regular">
          We are a virus that starts has something else!
          <br> and are still around because people can't warp it!
        </p>
      </v-col>
      <v-col
        class="mb-5" 
        cols="12"
      >
      <div>
        <br>
      <h2 class="subheading font-weight-bold mb-5">
        <p>About us.</p>
      </h2>
        <v-row 
          align="center"
          justify="center"
          class="dark"
          style="height: 100px;"
          >
            <v-card 
              v-for="(whats, i) in whatWe"
              :key="i"
              class="ma-2 pa-4"
              outlined
              shaped
              raised
              elevation="0.30"
              >
              {{ whats.text }}
            </v-card>
        </v-row>
        <br>
      </div>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
  export default {
    name: 'HelloWorld',

    data: () => ({
      whatWe: [
        {
          text: 'Mine shit',
        },
        {
          text: 'Refine shit'
        },
        {
          text: 'Build shit'
        },
        {
          text: 'Get wreaked in said built shit'
        },
        {
          text: 'Cry a little'
        },
        {
          text:'REPEAT!'
        },
      ],
    }),
  }
</script>
