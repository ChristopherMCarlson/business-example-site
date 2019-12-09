<template>
  <v-container>
    <v-row justify='space-around'>
      <v-col justify='center' cols='auto'>
        <v-card class="mx-auto" max-width="344">
          <v-img src="../assets/card1.jpg" height="200px"></v-img>
          <v-card-title>
            What We Do
          </v-card-title>
          <v-card-subtitle>
            How we can help you
          </v-card-subtitle>
          <v-card-actions>
            <v-btn text>Share</v-btn>
            <v-btn color="purple" text>
            Explore
            </v-btn>
            <v-spacer></v-spacer>
            <v-btn icon @click="card1 = !card1">
              <v-icon>{{ card1 ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
            </v-btn>
          </v-card-actions>
          <v-expand-transition>
            <div v-show="card1">
              <v-divider></v-divider>
              <v-card-text>
                  We offer simple but effective websites to small businesses at an affordable price.
              </v-card-text>
            </div>
          </v-expand-transition>
        </v-card>
      </v-col>
      <v-col justify='center' cols='auto'>
        <v-card class="mx-auto" max-width="344">
          <v-img src="../assets/card2.jpg" height="200px"></v-img>
          <v-card-title>
            Our Projects
          </v-card-title>
          <v-card-subtitle>
            What we've built
          </v-card-subtitle>
          <v-card-actions>
            <v-btn text>Share</v-btn>
            <v-btn color="purple" text>
            Explore
            </v-btn>
            <v-spacer></v-spacer>
            <v-btn icon @click="card2 = !card2">
              <v-icon>{{ card2 ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
            </v-btn>
          </v-card-actions>
          <v-expand-transition>
            <div v-show="card2">
              <v-divider></v-divider>
              <v-card-text>
                  Take a look at our other projects by clicking explore, where you'll be taken to our portfolio page.
              </v-card-text>
            </div>
          </v-expand-transition>
        </v-card>
      </v-col>
    </v-row>
    <v-row justify='space-around'>
      <v-col justify='center' cols='auto'>
        <div class="mapouter">
          <div class="gmap_canvas">
            <iframe width="600" height="500" id="gmap_canvas" src="https://maps.google.com/maps?q=1104%2011th%20Ave%20S%20Nampa%2C%20ID%2083651&t=&z=13&ie=UTF8&iwloc=&output=embed" frameborder="0" scrolling="no" marginheight="0" marginwidth="0"></iframe>
          </div>
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
  export default {
    data: () => ({
      card1: false,
      card2: false,
    }),
  }
</script>

<style>
  .mapouter{
    position:relative;
    text-align:right;
    height:500px;
    width:600px;
  }
  .gmap_canvas
  {overflow:hidden;
    background:none!important;
    height:500px;
    width:600px;
  }
  </style>