<template>
     <!-- <v-app style="
    background: #3A1C71;
    background: -webkit-linear-gradient(to right, #FFAF7B, #D76D77, #3A1C71);
    background: linear-gradient(to right, #FFAF7B, #D76D77, #3A1C71);
  "> -->
  <v-app style="
    background-color: whitesmoke;
  ">


    <Navbar />
    <v-content class="mx-4 mb-4">
      <router-view></router-view>
    </v-content>

    
  </v-app>
</template>

<script>

import Navbar from '@/components/Navbar';


export default {
  name: 'App',

  components: {
    Navbar
  },

  data: () => ({
    //
  }),
};
</script>
