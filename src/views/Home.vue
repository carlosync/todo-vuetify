<template>
 <div class="home">
   <v-card width="1000" class="mx-auto mt-5">
     <v-card-title>
       <h2 class="display-1">Clientes</h2>
     </v-card-title>
     <v-card-text>
       <v-form>
         <v-text-field label="Nome" prepend-icon="mdi-account-circle"/>
         <v-text-field label="Email" prepend-icon="mdi-email"/>
         <v-text-field :type="showPassword ? 'text' : 'password'" label="Senha:" 
                       prepend-icon="mdi-lock" :append-icon="showPassword ? 'mdi-eye' : 'mdi-eye-off'" 
                       @click:append="showPassword = !showPassword"/>
       </v-form>
     </v-card-text>
     <v-divider></v-divider>
     <v-card-actions>
       <v-btn color="primary">Salvar</v-btn>
     </v-card-actions>
   </v-card>
 </div>
</template>

<script>

export default {
  data(){
    return {
      showPassword: false
    }
  }
};
</script>

<style>
</style>
