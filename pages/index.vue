<template>
  <div>
    <v-row>
      <v-col class="ml-0">
        <v-carousel height="100vh" hide-delimiters>
          <v-carousel-item
            v-for="(item, i) in items"
            :key="i"
            :src="item.src"
            reverse-transition="fade-transition"
            transition="fade-transition"
          >
            <v-row align="center" justify="center" class="mt-16">
              <v-col>
                <v-row align="center" justify="center">
                  <v-col cols="12" md="6" xl="8" class="mt-16">
                    <h1 class="display-2 font-weight-bold mb-4 white--text font text-center">
                      Chefs Academy
                    </h1>
                    <h4 class="font-weight-light text-justify white--text font">
                      Chef Academy is a training Agency accredited since 2013
                      and issues certificates of qualification. Located in the
                      hub of the Abuja metropolis, the training is given in
                      compliance with high quality international standards. We
                      have Something for everyone From the amateur cooking
                      programs to complete CHEF TRAINING COURSES. Take a look at
                      the training courses we offer
                    </h4>
                    <v-row align="center" justify="center">
                    <v-btn
                      rounded
                      
                      large
                      dark
                      @click="$vuetify.goTo('#features')"
                      class="mt-5"
                    >
                      Find Courses
                      <v-icon class="ml-2">mdi-arrow-down</v-icon>
                    </v-btn>
                    </v-row>
                  </v-col>
                </v-row>
              </v-col>
            </v-row>
          </v-carousel-item>
        </v-carousel>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          src: '/land3.png',
        },
        {
          src: '/land4.png',
        },
        {
          src: '/land1.png',
        },
        {
          src: '/land2.png',
        },
      ],
    }
  },
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@600&display=swap');

.font{
 font-family: 'Poppins', sans-serif;
}

.section1 {
  width: 100vw;
  height: 100vh;
  overflow: hidden;
  background: #ffffff;
}

.section2 {
  width: 100vw;
  height: 100vh;
  overflow: hidden;
  background: #ffffff;
}



</style>
