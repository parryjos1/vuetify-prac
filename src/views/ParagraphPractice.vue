<template>
  <div class="home">
    <h1>Homepage</h1>

    <!-- Paragraphs, text & Color -->
    <p class="red white--text">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Maiores aut recusandae tempora libero adipisci in obcaecati corporis eius, nemo mollitia? Suscipit qui neque at eveniet. Veniam sapiente recusandae illum consectetur.</p>
    <p class="pink lighten-4 red--text text--darken-4">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nobis iure, neque quo sint nam provident vero? Nostrum, necessitatibus? Aperiam temporibus id nihil laudantium nam necessitatibus minima laborum perspiciatis quibusdam neque.</p>
    <h1 class="display-4">Massive Display</h1>
    <h4 class="display-1">smaller display</h4>
    <p class="headline">This is a headline</p>
    <p class="subheading .font-weight-bold">This is a subheading</p>
    <p class="caption">this is a caption</p>


    <!-- Buttons -->
        <v-btn class="pink white--text">click me</v-btn>
    <v-btn dark depressed color="pink">Click me</v-btn>
    <v-btn color="pink">Click me</v-btn>

    <v-btn depressed class="pink white--text">
      <v-icon left>mdi-email</v-icon>
      <span>email me</span>
    </v-btn>

    <v-btn depressed small class="pink white--text">
      <v-icon left small>mdi-email</v-icon>
      <span>email me</span>
    </v-btn>

    <v-btn depressed large class="pink white--text">
      <span>email me</span>
      <v-icon right large>mdi-email</v-icon>
    </v-btn>

    <v-btn depressed fab small dark color="purple">
      <v-icon>mdi-heart</v-icon>
    </v-btn>

         <v-btn text>Hello</v-btn>

    <!-- Breakpoints and visibility -->
    <v-btn class="hidden-md-and-down">Click me</v-btn>
    <v-btn class="hidden-md-and-up">Doing?</v-btn>
    <!-- Only being hidden for this range -->
    <v-btn class="hidden-sm-only">Button3</v-btn>




  </div>
</template>