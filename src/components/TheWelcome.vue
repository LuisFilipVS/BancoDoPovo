<script setup>

</script>

<template>
  <div class="base">
<v-sheet width="300" class="mx-auto sheet" >
  <v-form @submit.prevent class="form">
    <h2 style="text-align: center; margin-bottom: 20px;">BANCO DO POVO</h2>
    <div>
    <v-text-field
        v-model="firstName"
        :rules="rules"
        label="Login"
      ></v-text-field>
    </div>
    <v-text-field
        :type="'password'"
        placeholder="Senha"
      ></v-text-field>
    <div class="line3">
      <label for=""><a href="http://" target="_blank" rel="noopener noreferrer">Esqueci a senha</a></label> 
      <v-btn append-icon="$vuetify">
        Acessar
      </v-btn>

    </div>
      
  </v-form>
  
</v-sheet>
</div>  
</template>

<style scoped>
.base{
  height: 100vh;
  background-image: url("../assets/BGlogin.jpg");
  background-size: cover;
}
.form{
  padding-top: 25vh;
  border-radius: 10px;
  color: black; 
}
.sheet{
  background-color: transparent;
}

.line3{
  display: flex;
  justify-content: space-between;
}
</style>