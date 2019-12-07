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
  </v-container>
</template>
