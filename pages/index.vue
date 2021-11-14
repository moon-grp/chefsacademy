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
                    <h1
                      class="
                        display-2
                        font-weight-bold
                        mb-4
                        white--text
                        font
                        text-center
                      "
                    >
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
                        @click="$vuetify.goTo('#section2')"
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
    <div id="section2" class="ml-0">
      <v-row justify="center" class="mt-4">
        <h1 class="h1 font-weight-bold mb-4 font text-center">Chefs Academy</h1>
      </v-row>
      <v-row class="mt-2">
        <v-col cols="4">
          <v-card class="mx-auto" max-width="300" height="450">
            <v-img height="200" src="/c1.jpg"></v-img>

            <v-card-title class="font">Diploma in Culinary Art</v-card-title>

            <v-card-text class="font text-justify">
              Diploma in Culinary arts is a program specially designed for
              students who are interested in a global career in professional
              cooking
            </v-card-text>

            <v-card-actions>
              <v-btn
                color="#000000"
                dark
                class="ml-2 mb-2 text-capitalize"
                rounded
                @click="reserve"
              >
                learn more
              </v-btn>
            </v-card-actions>
          </v-card>
        </v-col>

        <v-col cols="4">
          <v-card class="mx-auto" max-width="300" height="450">
            <v-img height="200" src="/c2.jpeg"></v-img>

            <v-card-title class="font">Desserts & Pastries</v-card-title>

            <v-card-text class="font text-justify">
              Our course in dessert and pastry will allow you to showcase your
              creativity and passion for at boy teaching you the fundamentals  
            </v-card-text>

            <v-card-actions>
              <v-btn
                color="#000000"
                dark
                class="ml-2 mb-2 text-capitalize"
                rounded
                @click="reserve"
              >
                learn more
              </v-btn>
            </v-card-actions>
          </v-card>
        </v-col>

        <v-col cols="4">
          <v-card class="mx-auto" max-width="300" height="450" >
            <v-img height="200" src="/c2.png"></v-img>

            <v-card-title class="font">Continental Culinary Art</v-card-title>

            <v-card-text class="font text-justify" >
              Take your first steps into the Continental Culinary Art world with
              our Professional chefs to tutor you. With a practical
            </v-card-text>

            <v-card-actions>
              <v-btn
                color="#000000"
                dark
                class="ml-2 mb-2 text-capitalize"
                rounded
                @click="reserve"
              >
                learn more
              </v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </div>
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

.font {
  font-family: 'Poppins', sans-serif;
}

.section1 {
  width: 100vw;
  height: 100vh;
  overflow: hidden;
  background: #ffffff;
}

#section2 {
  width: 100vw;
  height: 100vh;
  overflow: hidden;
  background: ghostwhite;
}
</style>
