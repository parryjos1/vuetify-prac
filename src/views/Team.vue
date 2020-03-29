<template>
  <div class="team">
      <h1 class="subheading grey--text">Team</h1>
      <!-- <v-container fluid class="my-5"> -->
      <v-container class="my-5">
          <v-layout row wrap>
              <v-flex xs12 sm6 md4 lg3 v-for="person in team" :key="person.name">
                  <v-card flat class="text-center ma-3">
                      <v-responsive class="pt-4">
                          <!-- different to an image -->
                          <v-avatar size="100" class="grey lighten-2">
                              <img :src="person.avatar" alt="person avatar" srcset="">
                          </v-avatar>
                      </v-responsive>
                      <v-card-text>
                          <div class="subheading">{{person.name}}</div>
                          <div class="grey--text">{{person.role}}</div>
                      </v-card-text>
                      <!-- buttons go into a section called v-card-actions -->
                      <v-card-actions>
                          <v-btn text color="grey">
                              <v-icon small left>mdi-message</v-icon>
                              <span>message</span>
                          </v-btn>
                      </v-card-actions>
                  </v-card>
              </v-flex>
          </v-layout>
      </v-container>
  </div>
</template>

<script>
export default {

    data() {
        return {
            team: [
                { name: 'The Net Ninja', role: 'Web developer', avatar: '/avatar-1.jpeg' },
                { name: 'Ryu', role: 'Graphic designer', avatar: '/avatar-2.jpeg' },
                { name: 'Chun Li', role: 'Web developer', avatar: '/avatar-3.jpeg' },
                { name: 'Gouken', role: 'Social media maverick', avatar: '/avatar-4.jpeg' },
                { name: 'Yoshi', role: 'Sales guru', avatar: '/avatar-5.jpeg'}
            ]
        }
    }

}
</script>

<style>

</style>