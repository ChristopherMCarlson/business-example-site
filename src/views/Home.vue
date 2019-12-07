<template>
<v-container fluid>
  <v-row justify='center'>
    <v-col justify='center' cols='auto'>
        <v-img src='../assets/splashImage.jpg' height="70vh" max-width="100vw"></v-img>
    </v-col>
  </v-row>
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
                Leverage agile frameworks to provide a robust synopsis for high level overviews. Iterative approaches to corporate strategy foster collaborative thinking to further the overall value proposition. Organically grow the holistic world view of disruptive innovation via workplace diversity and empowerment.
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
                Bring to the table win-win survival strategies to ensure proactive domination. At the end of the day, going forward, a new normal that has evolved from generation X is on the runway heading towards a streamlined cloud solution. User generated content in real-time will have multiple touchpoints for offshoring.
            </v-card-text>
          </div>
        </v-expand-transition>
      </v-card>
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