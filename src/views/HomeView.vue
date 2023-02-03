<template>
  <v-container class="content" fluid>
    <v-parallax src="https://cdn.vuetifyjs.com/images/parallax/material2.jpg" height="500">
      <div class="row">
        <v-btn class="box1" variant="outlined" width="100" height="50" color="blue">
          Criar Conta
        </v-btn>
      </div>
      &nbsp;
      <div class="row1">
        <V-btn class="box2" variant="outlined" width="100" height="50" color="blue">
          Login
        </V-btn>
      </div>
      <div class="d-flex flex-column fill-height justify-center align-center text-white">
        <h1 class="title-home">
          Revivas Obras clássicas e inesquecíveis.
        </h1>
        <h4 class="subheading">
          Da década de 20 a 80.
        </h4>
      </div>
    </v-parallax>
    <v-img class="desktop" src=../assets/desktop.png height="550" width="550"></v-img>
    <v-divider class="line2"></v-divider>
    <v-row>
      <v-col cols="12" sm="6" md="4" lg="3" offset-lg="12">
        <v-img src="../assets/chefao.jpg" width="390" height="300"></v-img>
        <v-img src="../assets/007.jpg" width="390" height="222">
        </v-img>
      </v-col>
      <v-col>
        <v-img src="../assets/star-wars.jpg" width="390" height="321">
        </v-img>
      </v-col>
      <v-col>
        <v-img src="../assets/indiana-jones.jpg" width="390" height="321">
        </v-img>
      </v-col>
    </v-row>

    <v-divider class="line3"></v-divider>
  </v-container>
</template>

<script>

</script>


<style>
.v-main {
  background-color: #151515;
}

.row {
  pointer-events: none;
}

/* restaura a interação do toch e mouse a todos elementos "filhos", incluindo os botões e outros */
.row>* {
  pointer-events: auto;
}

.row:hover>[class*=box1] {
  background-color: whitesmoke;
}

.row1:hover>[class*=box2] {
  background-color: whitesmoke;
}

div>div {
  display: inline-block;
}

.box1 {
  font-size: 11px;
}

.text {
  color: white;
  font-size: 25px;
  font-family: 'Arial', sans-serif;
}

.line {
  color: white;
}

.line2 {
  color: white;
}

.line3 {
  color: white;
}

.title-home {
  font-weight: bold;
}
</style>