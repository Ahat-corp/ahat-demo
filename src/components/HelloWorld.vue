<template>
  <v-container>
    <v-row class="text-center">
      <v-col cols="12">
        <v-img
          :src="require('../assets/logo.svg')"
          class="my-5"
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
      <h2 class="headline font-weight-bold mb-3">
        <p>What we do.</p>
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
              class="ma-3 pa-6"
              outlined
              tile
              >
              {{ whats.text }}
            </v-card>
        </v-row>
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
          text:  'We mine! We also have orca boost, and everything',
        },
        {
          text: 'We love new and old players! All are welcome!'
        },
        {
          text: 'What are in all parts of production form basic T1 all the to T2'
        },

      ],



    }),
  }
</script>
