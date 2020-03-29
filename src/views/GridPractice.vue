<template>

  <div class="grid-ctn">

    <h1>grid</h1>

    <v-container class="my-5">
      <v-layout row wrap>
        <v-flex xs12 md6>
          <v-btn text block class="primary">1</v-btn>
        </v-flex>
        <v-flex xs4 md2>
          <v-btn text block class="primary">2</v-btn>
        </v-flex>
        <v-flex xs4 md2>
          <v-btn text block class="primary">3</v-btn>
        </v-flex>
        <v-flex xs4 md2>
          <v-btn text block class="primary">4</v-btn>
        </v-flex>
      </v-layout>

      <v-layout wrap justify-space-around>
        <v-flex xs4 md3 >
          <v-btn outlined block text >1</v-btn>
        </v-flex>
        <v-flex xs4 md3>
          <v-btn outlined block text >2</v-btn>
        </v-flex>
      </v-layout>

    </v-container>



  </div>

</template>