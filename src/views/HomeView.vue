<template>
  <div>
    <v-app-bar app class="blur" color="transparent" dark>
      <v-toolbar-title>GoldenMovies</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn color="secondary" text>Criar Conta</v-btn>
      <v-btn color="secondary" text>Entrar</v-btn>
    </v-app-bar>
    <!-- Parallax section -->
    <div>
      <v-parallax dark class="parallax" src="https://isquad.tv/wp-content/uploads/2018/08/Netflix-Background.jpg"
        style="filter: brightness(0.8) contrast(0.8) saturate(1.5);">
        <h1 class="title" style="filter: none; color: white;">Revivas obras clássicas e inesquecíveis.</h1>
        <p class="text" style="filter: none;">Revivas obras clássicas e inesquecíveis.</p>
      </v-parallax>
    </div>
    <br>
    <v-timeline direction="horizontal">
      <v-timeline-item>
        <template v-slot:opposite>
          Opposite content
        </template>
        <div>
          <div class="text-h6">Content title</div>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
            dolore magna aliqua.
          </p>
        </div>
      </v-timeline-item>

      <v-timeline-item>
        <template v-slot:opposite>
          Opposite content
        </template>
        <div>
          <div class="text-h6">Content title</div>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
            dolore magna aliqua.
          </p>
        </div>
      </v-timeline-item>

      <v-timeline-item>
        <template v-slot:opposite>
          Opposite content
        </template>
        <div>
          <div class="text-h6">Content title</div>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
            dolore magna aliqua.
          </p>
        </div>
      </v-timeline-item>
    </v-timeline>
    <!-- Main content section -->
    <br>
    <v-divider></v-divider>
    <br>
    <v-carousel
    cycle
    height="400"
    hide-delimiter-background
    show-arrows="hover"
  >
    <v-carousel-item
      v-for="(slide, i) in slides"
      :key="i"
    >
      <v-sheet
        :color="colors[i]"
        height="100%"
      >
        <div class="d-flex fill-height justify-center align-center">
          <div class="text-h2">
            {{ slide }} Slide
          </div>
        </div>
      </v-sheet>
    </v-carousel-item>
  </v-carousel>

  
  </div>
</template>


<script>
export default {
  data () {
  return {
        colors: [
          'indigo',
          'warning',
          'pink darken-2',
          'red lighten-1',
          'deep-purple accent-4',
        ],
        slides: [
          'First',
          'Second',
          'Third',
          'Fourth',
          'Fifth',
        ],
      }
    },
  }
</script>
<style>
  .original {
    color: white;
  }

  .line {
    color: white;
  }

  ul {
    display: flex;
    list-style: none;
    font-size: 20px;
  }

  li {
    margin-right: 30px;
    color: #b3b3b3;
  }

  .active {
    color: #fff;
    border-bottom: 2px solid #e50914;
  }

  .jumbotron {
    height: 90vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    color: #fff;
  }

  .mdi {
    height: 200%;
  }

  .main-content {
    margin-top: 50px;
    text-align: center;
    color: white;
    font-size: 20px;
  }

  h2 {
    font-size: 30px;
    margin-bottom: 30px;
  }

  .card-container {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
  }

  .card {
    width: 23%;
    margin-bottom: 20px;
  }

  .card img {
    width: 100%;
    border-radius: 5px;
  }

  .icons img {
    width: 100%;
    border-radius: 5px;
  }

  .parallax {
    height: 500px;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    color: #fff;
  }

  .parallax h1 {
    font-size: 50px;
    margin-bottom: 20px;
  }

  .parallax p {
    font-size: 30px;
    margin-bottom: 30px;
  }

  @media screen and (max-width: 600px) {
    .card {
      width: 48%;
    }

    .parallax h1 {
      font-size: 30px;
    }

    .parallax p {
      font-size: 20px;
    }

    .text-h6 {
      font-size: 18px;
    }

    .main-content {
      font-size: 16px;
    }

    h2 {
      font-size: 20px;
    }

    .pt-container {
      display: flex;
    }

    .pt-0 {
      flex-grow: 1;
      flex-basis: 0;
    }
  }
</style>