

<template>
    <nav>
        <v-toolbar flat app >
        <v-app-bar-nav-icon class="grey--text" @click="drawer = !drawer"></v-app-bar-nav-icon>
            <v-toolbar-title class="text-uppercase grey--text">
                <span class="font-weight-light">Todo</span>
                <span>Nina</span>
            </v-toolbar-title>
            <v-spacer></v-spacer>    
            <v-btn text color="grey">
                <span>Sign Out</span>
                <v-icon right>mdi-exit-to-app</v-icon>
            </v-btn>


        </v-toolbar>


        <v-navigation-drawer v-model="drawer" app class="primary">
            <v-list>
                <v-list-tile v-for="link in links" :key="link.text" router :to="link.route">
                    <v-list-tile-action>
                        <v-icon class="white--text">mdi-{{ link.icon }}</v-icon>
                    </v-list-tile-action>
                    <v-list-tile-content>
                        <v-list-tile-title class="white--text">{{ link.text }}</v-list-tile-title>
                    </v-list-tile-content>
                </v-list-tile>
            </v-list>
        </v-navigation-drawer>
    </nav>
</template>

<script>

export default {
    data() {
        return {
            drawer: false,
            links: [
                {icon: 'diamond-stone', text: 'Dashboard', route: '/'},
                {icon: 'disk-player', text: 'My Projects', route: '/projects'},
                {icon: 'dropbox', text: 'Team', route: '/team'}
            ],
        }
    }

}
</script>

<style>

</style>