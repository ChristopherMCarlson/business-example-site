<template>
  <v-container fluid fill-height class="home-hero">
    <v-row>
      <v-col>
        <v-row justify='space-around' align="center">
          <v-col justify='center' cols='auto'>
            <div class="display-3 font-weight-black white--text text-xs-center">MODERN WEBSITES</div>
          </v-col>
        </v-row>
        <v-row justify='space-around' align="center">
          <v-col justify='center' cols='auto'>
            <div class="display-3 font-weight-black white--text text-xs-center mb-3">FOR MODERN BUSINESSES</div>
          </v-col>
        </v-row>
        <v-row justify='center' align="center">
          <v-col justify='center' cols='auto'>
            <v-btn large color="normal">Learn More</v-btn>
          </v-col>
          <v-col justify='center' cols='auto'>
            <v-btn large color="primary">Book Now</v-btn>
          </v-col>
        </v-row>
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

<style scoped>
  .home-hero {
      background: url('../assets/card2.jpg');
      background-size: cover;
      width: 100%;
      height: 100%;
  }
  </style>