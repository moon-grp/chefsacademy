<template>
  <div>
         <SfBanner
        title="Services we offer"
        background=""
        image="https://res.cloudinary.com/sparaclet-inc/image/upload/v1647168959/chefsacademy/photo5868253566903368401_wsnhob.jpg"
      />
      <v-container>
           <v-row class="">
              <v-col cols="4" class="mx-auto">
                <v-card class="mx-auto" width="280" outlined elevation="2">
                  <v-img
                    height="180"
                    src="https://res.cloudinary.com/sparaclet-inc/image/upload/v1647168959/chefsacademy/photo5868253566903368401_wsnhob.jpg"
                  ></v-img>

                  <v-card-title class="fntx"
                    >Outdoor cateering</v-card-title
                  >

                

                  <v-card-actions>
                    <v-btn
                      color=""
                      class="text-capitalize"
                      outlined
                      to="/courses/diploma-culinary-art"
                    >
                      learn more
                    </v-btn>
                  </v-card-actions>
                </v-card>
              </v-col>

               <v-col cols="4" class="mx-auto">
                <v-card class="mx-auto" width="280" outlined elevation="2">
                  <v-img
                    height="180"
                    src="https://res.cloudinary.com/sparaclet-inc/image/upload/v1647168958/chefsacademy/photo5868253566903368402_ihwxga.jpg"
                  ></v-img>

                  <v-card-title class="fntx"
                    >Bartending</v-card-title
                  >

                

                  <v-card-actions>
                    <v-btn
                      color=""
                      class="text-capitalize"
                      outlined
                      to="/courses/diploma-culinary-art"
                    >
                      learn more
                    </v-btn>
                  </v-card-actions>
                </v-card>
              </v-col>

              
               <v-col cols="4" class="mx-auto">
                <v-card class="mx-auto" width="280" outlined elevation="2">
                  <v-img
                    height="180"
                    src="https://res.cloudinary.com/sparaclet-inc/image/upload/v1647168961/chefsacademy/photo5868253566903368399_gc0jhr.jpg"
                  ></v-img>

                  <v-card-title class="fntx"
                    >kitchen setup</v-card-title
                  >
                  <v-card-actions>
                    <v-btn
                      color=""
                      class="text-capitalize"
                      outlined
                      to="/courses/diploma-culinary-art"
                    >
                      learn more
                    </v-btn>
                  </v-card-actions>
                </v-card>
              </v-col>

                   <v-col cols="4" class="mx-auto">
                <v-card class="mx-auto" width="280" outlined elevation="2">
                  <v-img
                    height="180"
                    src="https://res.cloudinary.com/sparaclet-inc/image/upload/v1647168958/chefsacademy/photo5868253566903368398_oqq1iv.jpg"
                  ></v-img>

                  <v-card-title class="fntx"
                    >Menu Engineering</v-card-title
                  >
                  <v-card-actions>
                    <v-btn
                      color=""
                      class="text-capitalize"
                      outlined
                      to="/courses/diploma-culinary-art"
                    >
                      learn more
                    </v-btn>
                  </v-card-actions>
                </v-card>
              </v-col>

                   <v-col cols="4" class="mx-auto">
                <v-card class="mx-auto" width="280" outlined elevation="2">
                  <v-img
                    height="180"
                    src="https://res.cloudinary.com/sparaclet-inc/image/upload/v1647168960/chefsacademy/photo5868253566903368400_cut7h7.jpg"
                  ></v-img>

                  <v-card-title class="fntx"
                    >Chef recruitment</v-card-title
                  >
                  <v-card-actions>
                    <v-btn
                      color=""
                      class="text-capitalize"
                      outlined
                      to="/courses/diploma-culinary-art"
                    >
                      learn more
                    </v-btn>
                  </v-card-actions>
                </v-card>
              </v-col>
           </v-row>
      </v-container>
  </div>
</template>

<script>
import { SfBanner } from '@storefront-ui/vue'
export default {
  components: {
    SfBanner,
  },
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Urbanist:wght@500&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@600&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Dancing+Script&family=Urbanist:wght@500&display=swap');
.sf-banner {
  height: 100vh;
  font-family: 'Urbanist', sans-serif;
}
.section2 {
  height: 100%;
}

.fntx {
  font-family: 'Urbanist', sans-serif;
}

.fntx-home {
  font-family: 'Dancing Script', cursive;
  font-size: 40px;
}

.sf-banner__title {
  font-family: 'Poppins', sans-serif;
  font-size: 50px;
  font-weight: bold;


}
.sf-banner__description {
  font-family: 'Urbanist', sans-serif;
  font-size: 20px;
  font-weight: bold;
}

@media screen and (max-width: 992px) {
  .sf-banner {
    font-family: 'Poppins', sans-serif;
  }
}

/* On screens that are 600px wide or less, make the columns stack on top of each other instead of next to each other */
@media screen and (max-width: 600px) {
  .sf-banner {
    font-family: 'Poppins', sans-serif;
  }

  .sf-banner__title {
    margin-top: 50%;
  }
}
</style>
