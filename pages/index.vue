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
                        x-large
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

    <!--sec 2 -->
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
          <v-card class="mx-auto" max-width="300" height="450">
            <v-img height="200" src="/c2.png"></v-img>

            <v-card-title class="font">Continental Culinary Art</v-card-title>

            <v-card-text class="font text-justify">
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

    <!--sec3 -->
    <div id="section3">
      <v-row justify="center" class="mt-4">
        <h1 class="h1 font-weight-bold mb-4 font text-center text-capitalize">
          why Chefs Academy?
        </h1>
      </v-row>
      <v-row class="mt-6 ml-0">
        <v-col class="" cols="3">
          <v-row justify="center">
            <v-icon color="#6592E6" x-large> mdi-vector-combine </v-icon>
          </v-row>

          <v-row
            justify="center"
            class="text-capitalize mt-10 font-weight-medium font h1"
          >
            experience!
          </v-row>
          <v-row
            justify="center font-weight-medium font h1"
            class="text-capitalize"
          >
            over 600
          </v-row>
          <v-row
            justify="center font-weight-medium font h1"
            class="text-capitalize"
          >
            students trained
          </v-row>
        </v-col>

        <v-col class="" cols="3">
          <v-row justify="center">
            <v-icon color="#6592E6" x-large> mdi-account-group </v-icon>
          </v-row>

          <v-row
            justify="center"
            class="text-capitalize mt-10 font-weight-medium font h1"
          >
            Rated among top
          </v-row>
          <v-row
            justify="center font-weight-medium font h1"
            class="text-capitalize"
          >
            10 Culinary
          </v-row>
          <v-row
            justify="center font-weight-medium font h1"
            class="text-capitalize"
          >
            School in Africa
          </v-row>
        </v-col>

        <v-col class="" cols="3">
          <v-row justify="center">
            <v-icon color="#6592E6" x-large> mdi-file-document-edit </v-icon>
          </v-row>

          <v-row
            justify="center"
            class="text-capitalize mt-10 font-weight-medium font h1"
          >
            Flexible training
          </v-row>
          <v-row
            justify="center font-weight-medium font h1"
            class="text-capitalize"
          >
            schedule
          </v-row>
        </v-col>

        <v-col class="" cols="3">
          <v-row justify="center">
            <v-icon color="#6592E6" x-large> mdi-shape-square-plus </v-icon>
          </v-row>

          <v-row
            justify="center"
            class="text-capitalize mt-10 font-weight-medium font h1"
          >
            Individual
          </v-row>
          <v-row
            justify="center font-weight-medium font h1"
            class="text-capitalize"
          >
            learning space
          </v-row>
        </v-col>
      </v-row>
    </div>

    <!--sec 4 -->
    <div id="section4">
      <v-row justify="center" class="mt-4">
        <h1 class="h1 font-weight-bold mb-4 font text-center text-capitalize">
          Some of Our chefs
        </h1>
      </v-row>

      <v-row class="mt-6">
        <v-col cols="6">
          <v-card class="ml-auto" max-width="300">
            <v-img height="280" src="/chf1.jpg"></v-img>

            <v-card-title class="font text-capitalize">
              <v-row justify="center" class="h1"> Chef IG </v-row>
            </v-card-title>
            <v-card-subtitle class="mt-1">
              <v-row justify="center" class="h1"> Head chef </v-row>
            </v-card-subtitle>

            <v-card-text class="font">
              An excellent chef with over ten years of experience.
            </v-card-text>

            <v-row justify="center">
              <v-card-actions>
                <v-icon color="#6592E6" x-large class="mx-auto">
                  mdi-instagram
                </v-icon>
                <v-icon color="#6592E6" x-large class="mx-auto"
                  >> mdi-twitter
                </v-icon>
                <v-icon color="#6592E6" x-large class="mx-auto"
                  >> mdi-facebook
                </v-icon>
              </v-card-actions>
            </v-row>
          </v-card>
        </v-col>

        <v-col cols="6">
          <v-card class="mr-auto" max-width="300">
            <v-img height="280" src="/chf2.jpeg"></v-img>

            <v-card-title class="font text-capitalize">
              <v-row justify="center" class="h1"> Chef China </v-row>
            </v-card-title>
            <v-card-subtitle class="mt-1">
              <v-row justify="center" class="h1"> Pastry Chef </v-row>
            </v-card-subtitle>

            <v-card-text class="font">
              Don't mess with this woman when it comes to variety of pastries.
            </v-card-text>

            <v-row justify="center">
              <v-card-actions>
                <v-icon color="#6592E6" x-large class="mx-auto">
                  mdi-instagram
                </v-icon>
                <v-icon color="#6592E6" x-large class="mx-auto"
                  >> mdi-twitter
                </v-icon>
                <v-icon color="#6592E6" x-large class="mx-auto"
                  >> mdi-facebook
                </v-icon>
              </v-card-actions>
            </v-row>
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

#section3 {
  width: 100vw;
  height: 50vh;
  overflow: hidden;
  background: ghostwhite;
}

#section4 {
  width: 100vw;
  height: 110vh;
  overflow: hidden;
  background: ghostwhite;
}
</style>
