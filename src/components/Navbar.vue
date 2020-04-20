<template>
  <nav>
      <v-toolbar flat app>
        <v-app-bar-nav-icon class="grey--text" @click="drawer = !drawer"></v-app-bar-nav-icon>
         <v-toolbar-title class="text-uppercase grey--text">
             <span class="font-weight-light">Minhas</span>
             <span> Finanças</span>
         </v-toolbar-title>
         <v-spacer></v-spacer>
         <v-btn flat color="grey lighten-4">
             <span>Sign Out</span>
             <v-icon right>mdi-exit-to-app</v-icon>
         </v-btn>
      </v-toolbar>

    <v-navigation-drawer app v-model="drawer" temporary class="primary">
        <p>Dashboard</p>
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
}
</script>

<style>

</style>