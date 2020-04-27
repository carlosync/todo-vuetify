<template>
  <nav>
      <v-app-bar color="deep-purple" dark="" app>
        <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>
         <v-toolbar-title class="text-uppercase grey-text">
             <span class="font-weight-light">Minhas</span>
             <span> Finanças</span>
         </v-toolbar-title>
         <v-spacer></v-spacer>
         <v-btn class="ma-2" outlined color="grey lighten-5">
             <span>Sign Out</span>
             <v-icon right>mdi-exit-to-app</v-icon>
         </v-btn>
      </v-app-bar>

    <v-navigation-drawer app v-model="drawer" temporary>
        <v-list nav dense>
            <v-list-item-group  active-class="deep-purple--text text--accent-4">
                <v-list-item href="/">
                    <v-list-item-icon>
                        <v-icon>mdi-view-dashboard</v-icon>
                    </v-list-item-icon>
                    <v-list-item-title>Dashboard</v-list-item-title>
                </v-list-item>
                <v-list-item href="/about">
                    <v-list-item-icon>
                        <v-icon>mdi-help-box</v-icon>
                    </v-list-item-icon>
                    <v-list-item-title>Sobre</v-list-item-title>
                </v-list-item>
            </v-list-item-group>
        </v-list>
    </v-navigation-drawer>
  </nav>
</template>

<script>
export default {

    data(){
        return{
            drawer: false
        }
    }
};
</script>

<style>

</style>