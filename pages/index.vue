<template>
  <div>
    <!--  <v-row class="section1">
      <v-carousel height="100vh" hide-delimiters :show-arrows="false">
        <v-carousel-item
          src="/jbt.jpg"
          reverse-transition="fade-transition"
          transition="fade-transition"
        >
          <v-row align="center" justify="center" class="mt-16">
            <v-col>
              <v-row align="center" justify="center">
                <v-col cols="12" md="6" xl="8">
                  <h1 class="display-2 font-weight-bold mb-4 font">
                    Professional Culinary School
                  </h1>
                  <v-row align="center" justify="center">
                    <h5 class="font-weight-light ">
                      Lorem ipsum dolor sit amet consectetur 
                      adipisicing elit. Maiores porro voluptatibus
                      delectus nam optio harum!
                    </h5>
                  </v-row>
                  <v-row align="center" justify="center">
                    <v-btn
                      rounded
                      outlined
                      large
                      color="#f2874a"
                      @click="$vuetify.goTo('#features')"
                      class="mt-5"
                    >
                      view courses
                      <v-icon class="ml-2">mdi-arrow-down</v-icon>
                    </v-btn>
                  </v-row>
                </v-col>
              </v-row>
            </v-col>
          </v-row>

              <v-row align="center" justify="center" >
            <v-col cols="12" class="">
              <v-row align="center" class="ml-6">
                <v-col cols="12" md="6" xl="8">
                  <h1 class="display-2 font-weight-bold mb-4 font">
                    Professional Culinary School
                  </h1>
                  <h5 class="font-weight-light">
                    Lorem ipsum dolor sit amet consectetur <br />
                    adipisicing elit. Maiores porro voluptatibus <br />
                    delectus nam optio harum!
                  </h5>
                  <v-btn
                    rounded
                    outlined
                    large
                    color="#f2874a"
                    @click="$vuetify.goTo('#features')"
                    class="mt-5"
                  >
                    view courses
                    <v-icon class="ml-2">mdi-arrow-down</v-icon>
                  </v-btn>
                </v-col>
              </v-row>
            </v-col>
          </v-row> 
        </v-carousel-item>
      </v-carousel>
    </v-row> -->

    <v-row align="center" justify="start" class="section1">
      <v-carousel height="100vh" hide-delimiters :show-arrows="false">
        <v-carousel-item
          src="jbt.jpg"
          reverse-transition="fade-transition"
          transition="fade-transition"
          gradient="to top right, rgba(100,115,201,.33), rgba(25,32,72,.7)"
        >
          <v-container>
            <v-col cols="10">
              <v-row align="start" justify="start" class="wordspace">
                <v-col cols="12" md="6" xl="8">
                  <h1 class="display-2 font-weight-bold mb-4 font">
                    Chefs Academy
                  </h1>
                  <h1 class="font-weight-light font">
                    Master the act of pastry, Baking, <br />
                    cookery and more. Skils that will take your career to the
                    next level.
                  </h1>
                  <v-btn
                    rounded
                    outlined
                    large
                    @click="$vuetify.goTo('#courses')"
                    class="mt-5"
                    color=""
                  >
                    view courses
                    <v-icon class="ml-2">mdi-arrow-down</v-icon>
                  </v-btn>
                </v-col>
              </v-row>
            </v-col>
          </v-container>
        </v-carousel-item>
      </v-carousel>
      <!--    <v-container>
        <v-col cols="10">
          <v-row align="start" justify="start">
            <v-col cols="12" md="6" xl="8">
              <h1 class="display-2 font-weight-bold mb-4">Chefs Academy</h1>
              <h1 class="font-weight-light">
                Master the act of pastry, Baking, <br />
                cookery and more.  
                Skils that will take your career to the next level.
              </h1>
              <v-btn
                rounded
                outlined
                large
                @click="$vuetify.goTo('#features')"
                class="mt-5"
              >
                view courses
                <v-icon class="ml-2">mdi-arrow-down</v-icon>
              </v-btn>
            </v-col>
          </v-row>
        </v-col>

      </v-container> -->
    </v-row>

    <v-row class="mb-4" id="courses">
      <v-container>
        <v-row class="h1">
          <p class="font-weight-bold h1 fnt-x">Courses</p>
        </v-row>
        <v-row class="">
          <v-col cols="4">
            <v-card class="" width="280" outlined elevation="6">
              <v-img height="180" src="newL.jpg"></v-img>

              <v-card-title class="fntc"
                >Diploma<br />In Culinary Art</v-card-title
              >

              <v-row>
                <v-col class="text-h2" cols="6">
                  <v-list-item two-line>
                    <v-list-item-content>
                      <v-list-item-title class="fntc">
                        Tution
                      </v-list-item-title>
                      <v-list-item-subtitle>₦ 365,000</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-col>

                <v-col class="" cols="6">
                  <v-list-item two-line>
                    <v-list-item-content>
                      <v-list-item-title class="fntc">
                        Duration
                      </v-list-item-title>
                      <v-list-item-subtitle>12 weeks</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-col>
              </v-row>

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

          <v-col cols="4">
            <v-card class="" width="280" outlined elevation="6">
              <v-img height="180" src="ad.jpg"></v-img>

              <v-card-title class="fntc"
                >Advance Diploma <br />in Culinary Art</v-card-title
              >

              <v-row>
                <v-col class="text-h2" cols="6">
                  <v-list-item two-line>
                    <v-list-item-content>
                      <v-list-item-title class="fntc">
                        Tution
                      </v-list-item-title>
                      <v-list-item-subtitle>₦ 550,000</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-col>

                <v-col class="" cols="6">
                  <v-list-item two-line>
                    <v-list-item-content>
                      <v-list-item-title class="fntc">
                        Duration
                      </v-list-item-title>
                      <v-list-item-subtitle>12 weeks</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-col>
              </v-row>

              <v-card-actions>
                <v-btn
                  color=""
                  class="text-capitalize"
                  outlined
                  to="/courses/advance-diploma-culinary-art"
                >
                  learn more
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-col>

          <v-col cols="4">
            <v-card class="" width="280" outlined elevation="6">
              <v-img height="180" src="pd.jpg"></v-img>

              <v-card-title class="fntc"
                >Professional Diploma<br />In Culinary Art</v-card-title
              >

              <v-row>
                <v-col class="text-h2" cols="6">
                  <v-list-item two-line>
                    <v-list-item-content>
                      <v-list-item-title class="fntc">
                        Tution
                      </v-list-item-title>
                      <v-list-item-subtitle>₦ 1,000,000</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-col>

                <v-col class="" cols="6">
                  <v-list-item two-line>
                    <v-list-item-content>
                      <v-list-item-title class="fntc">
                        Duration
                      </v-list-item-title>
                      <v-list-item-subtitle>nine months</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-col>
              </v-row>

              <v-card-actions>
                <v-btn
                  color=""
                  class="text-capitalize"
                  outlined
                  to="/courses/professional-diploma-culinary-art"
                >
                  learn more
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-row>

    <v-row class="mb-4">
      <v-container>
        <v-row class="">
          <v-col cols="4">
            <v-card class="" width="280" outlined elevation="6">
              <v-img height="180" src="pa.jpg"></v-img>

              <v-card-title class="fntc"
                >Desserts /<br />Pastary Art</v-card-title
              >

              <v-row>
                <v-col class="text-h2" cols="6">
                  <v-list-item two-line>
                    <v-list-item-content>
                      <v-list-item-title class="fntc">
                        Tution
                      </v-list-item-title>
                      <v-list-item-subtitle>₦ 355,000</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-col>

                <v-col class="" cols="6">
                  <v-list-item two-line>
                    <v-list-item-content>
                      <v-list-item-title class="fntc">
                        Duration
                      </v-list-item-title>
                      <v-list-item-subtitle>4 weeks</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-col>
              </v-row>

              <v-card-actions>
                <v-btn
                  color=""
                  class="text-capitalize"
                  outlined
                  to="/courses/pastry-dessert-art"
                >
                  learn more
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-col>

          <v-col cols="4">
            <v-card class="" width="280" outlined elevation="6">
              <v-img height="180" src="cc.jpg"></v-img>

              <v-card-title class="fntc"
                >Continental <br />Culinary Art</v-card-title
              >

              <v-row>
                <v-col class="text-h2" cols="6">
                  <v-list-item two-line>
                    <v-list-item-content>
                      <v-list-item-title class="fntc">
                        Tution
                      </v-list-item-title>
                      <v-list-item-subtitle>₦ 355,000</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-col>

                <v-col class="" cols="6">
                  <v-list-item two-line>
                    <v-list-item-content>
                      <v-list-item-title class="fntc">
                        Duration
                      </v-list-item-title>
                      <v-list-item-subtitle>5 weeks</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-col>
              </v-row>

              <v-card-actions>
                <v-btn
                  color=""
                  class="text-capitalize"
                  outlined
                  to="/courses/continental-culinary"
                >
                  learn more
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-col>

          <v-col cols="4">
            <v-card class="" width="280" outlined elevation="6">
              <v-img height="180" src="pz.jpg"></v-img>

              <v-card-title class="fntc"
                >Healthy<br />living cuisine</v-card-title
              >

              <v-row>
                <v-col class="text-h2" cols="6">
                  <v-list-item two-line>
                    <v-list-item-content>
                      <v-list-item-title class="fntc">
                        Tution
                      </v-list-item-title>
                      <v-list-item-subtitle>₦ 280,000</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-col>

                <v-col class="" cols="6">
                  <v-list-item two-line>
                    <v-list-item-content>
                      <v-list-item-title class="fntc">
                        Duration
                      </v-list-item-title>
                      <v-list-item-subtitle>5 weeks</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-col>
              </v-row>

              <v-card-actions>
                <v-btn
                  color=""
                  class="text-capitalize"
                  outlined
                  to="/courses/healthy-living"
                >
                  learn more
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-row>

    <v-row class="">
      <v-container>
        <v-row class="">
          <v-col cols="4">
            <v-card class="" width="280" outlined elevation="6">
              <v-img height="180" src="ca.jpg"></v-img>

              <v-card-title class="fntc">Cake <br />Baking Art</v-card-title>

              <v-row>
                <v-col class="text-h2" cols="6">
                  <v-list-item two-line>
                    <v-list-item-content>
                      <v-list-item-title class="fntc">
                        Tution
                      </v-list-item-title>
                      <v-list-item-subtitle>₦ 300,000</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-col>

                <v-col class="" cols="6">
                  <v-list-item two-line>
                    <v-list-item-content>
                      <v-list-item-title class="fntc">
                        Duration
                      </v-list-item-title>
                      <v-list-item-subtitle>4 weeks</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-col>
              </v-row>

              <v-card-actions>
                <v-btn
                  color=""
                  class="text-capitalize"
                  outlined
                  to="courses/cake-baking-art"
                >
                  learn more
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-col>

          <v-col cols="4">
            <v-card class="" width="280" outlined elevation="6">
              <v-img height="180" src="ac.jpg"></v-img>

              <v-card-title class="fntc"
                >African <br />Cuisine Art</v-card-title
              >

              <v-row>
                <v-col class="text-h2" cols="6">
                  <v-list-item two-line>
                    <v-list-item-content>
                      <v-list-item-title class="fntc">
                        Tution
                      </v-list-item-title>
                      <v-list-item-subtitle>₦ 180,000</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-col>

                <v-col class="" cols="6">
                  <v-list-item two-line>
                    <v-list-item-content>
                      <v-list-item-title class="fntc">
                        Duration
                      </v-list-item-title>
                      <v-list-item-subtitle>3 weeks</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-col>
              </v-row>

              <v-card-actions>
                <v-btn
                  color=""
                  class="text-capitalize"
                  outlined
                  to="courses/african-cuisine"
                >
                  learn more
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-col>

          <v-col cols="4">
            <v-card class="" width="280" outlined elevation="6">
              <v-img height="180" src="jnr.jpg"></v-img>

              <v-card-title class="fntc"
                >Chef's <br />Academy junior</v-card-title
              >

              <v-row>
                <v-col class="text-h2" cols="6">
                  <v-list-item two-line>
                    <v-list-item-content>
                      <v-list-item-title class="fntc"> </v-list-item-title>
                      <v-list-item-subtitle></v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-col>

                <v-col class="" cols="6">
                  <v-list-item two-line>
                    <v-list-item-content>
                      <v-list-item-title class="fntc"> </v-list-item-title>
                      <v-list-item-subtitle></v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-col>
              </v-row>

              <v-card-actions>
                <v-btn
                  color=""
                  class="text-capitalize"
                  outlined
                  to="courses/chefs-junior"
                >
                  learn more
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-col>

          <v-col cols="4">
            <v-card class="" width="280" outlined elevation="6">
              <v-img height="180" src="ent.jpg"></v-img>

              <v-card-title class="fntc"
                >Food Entrepreneurship <br />and restaurant<br />
                management</v-card-title
              >

              <v-row>
                <v-col class="text-h2" cols="6">
                  <v-list-item two-line>
                    <v-list-item-content>
                      <v-list-item-title class="fntc">
                        Tution
                      </v-list-item-title>
                      <v-list-item-subtitle>₦ 200,000</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-col>

                <v-col class="" cols="6">
                  <v-list-item two-line>
                    <v-list-item-content>
                      <v-list-item-title class="fntc">
                        Duration
                      </v-list-item-title>
                      <v-list-item-subtitle>2 weeks</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-col>
              </v-row>

              <v-card-actions>
                <v-btn
                  color=""
                  class="text-capitalize"
                  outlined
                  to="/courses/management"
                >
                  learn more
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-row>

    
    <div id="section4">
      <v-row justify="center" class="mt-4">
        <h1 class="h1 font-weight-bold mb-4 font text-center text-capitalize">
          Some of Our chefs
        </h1>
      </v-row>

      <v-row class="mt-6">
        <v-col cols="6">
          <v-card class="ml-auto" max-width="300" elevation="10">
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
          <v-card class="mr-auto" max-width="300" elevation="10">
            <v-img height="280" src="/chf2.jpg"></v-img>

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



     <div id="section5">
      <v-row justify="center" class="mt-4">
        <h1 class="h1 font-weight-bold mb-4 font text-center text-capitalize">
          My Experience at Chefs Academy
        </h1>
      </v-row>

      <v-row>
        <v-carousel
          cycle
          height="400"
          hide-delimiter-background
          show-arrows-on-hover
        >
          <v-carousel-item>
            <v-row justify="center" class="mt-8">
              <v-avatar color="primary" size="164">
                <img src="/grad3.jpg" />
              </v-avatar>
            </v-row>
            <v-row justify="center" class="mt-4">
              <div class="text-center mx-auto font mt-4">
                The professionalism at Chef's Academy is top notch and the
                quality <br />
                of services rendered are highly commendable. I'd recommend
                Chef's Academy not just for the value one gets but also for the
                amazing <br />
                learning experience that stays with you long after the end of
                the program
              </div>
            </v-row>
            <v-row justify="center" class="mt-4">
              <div class="text-center mx-auto font mt-4 overline">Amaka</div>
            </v-row>

            <v-row justify="center" class="mt-2">
              <div class="text-center mx-auto font mt-4 h4">GRADUATE</div>
            </v-row>
          </v-carousel-item>

          <v-carousel-item>
            <v-row justify="center" class="mt-8">
              <v-avatar color="primary" size="164">
                <img src="/grd1.jpg" />
              </v-avatar>
            </v-row>
            <v-row justify="center" class="mt-4">
              <div class="text-center mx-auto font mt-4">
                Training at Chef's Academy is the highlight of my professional
                career so far.<br />
                The wealth of knowledge taught and the practical application
                will launch anyone<br />
                who desires to go into the culinary world from a novice to a
                professional per excellence.
              </div>
            </v-row>
            <v-row justify="center" class="mt-4">
              <div class="text-center mx-auto font mt-4 overline">
                Anselm Ekere
              </div>
            </v-row>

            <v-row justify="center" class="mt-2">
              <div class="text-center mx-auto font mt-4 h4">GRADUATE</div>
            </v-row>
          </v-carousel-item>

          <v-carousel-item>
            <v-row justify="center" class="mt-8">
              <v-avatar color="primary" size="164">
                <img src="/grad2.jpg" />
              </v-avatar>
            </v-row>
            <v-row justify="center" class="mt-4">
              <div class="text-center mx-auto font mt-4">
                The professionalism at Chef's Academy is top notch and the
                quality of services rendered are highly commendable.<br />
                I'd recommend Chef's Academy not just for the value one gets but
                also for the amazing learning<br />
                experience that stays with you long after the end of the program
              </div>
            </v-row>
            <v-row justify="center" class="mt-4">
              <div class="text-center mx-auto font mt-4 overline">Tokunbo</div>
            </v-row>

            <v-row justify="center" class="mt-2">
              <div class="text-center mx-auto font mt-4 h4">GRADUATE</div>
            </v-row>
          </v-carousel-item>
        </v-carousel>
      </v-row>
    </div>

  <div id="section6">
      <v-row justify="center" class="mt-4">
        <h1 class="h1 font-weight-bold mb-4 font text-center text-capitalize">
          Some of Our Clients
        </h1>
      </v-row>

      <v-row class="mt-6 ml-0">
        <v-col cols="2">
          <v-img contain height="100" max-width="150" src="/hlt.svg"></v-img>
        </v-col>
        <v-col cols="2">
          <v-img height="100" contain max-width="150" src="nab.jpg"></v-img>
        </v-col>
        <v-col cols="2">
          <v-img contain height="100" max-width="150" src="jbc.png"></v-img>
        </v-col>
        <v-col cols="2">
          <v-img contain height="100" max-width="150" src="/fis.jpg"></v-img>
        </v-col>
        <v-col cols="2">
          <v-img contain height="100" max-width="150" src="cam.jpg"></v-img>
        </v-col>
        <v-col cols="2" class="">
          <v-img contain height="100" max-width="150" src="cer.jpg"></v-img>
        </v-col>
      </v-row>
    </div>


    <!--sec 2 
    <div id="section2" class="ml-0">
      <v-row justify="center" class="mt-4">
        <h1 class="h1 font-weight-bold mb-4 font text-center">Chefs Academy</h1>
      </v-row>
      <v-row class="mt-2">
        <v-col cols="4">
          <v-card class="mx-auto" max-width="300" height="450" elevation="10">
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
          <v-card class="mx-auto" max-width="300" height="450" elevation="10">
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
          <v-card class="mx-auto" max-width="300" height="450" elevation="10">
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


    <div id="section4">
      <v-row justify="center" class="mt-4">
        <h1 class="h1 font-weight-bold mb-4 font text-center text-capitalize">
          Some of Our chefs
        </h1>
      </v-row>

      <v-row class="mt-6">
        <v-col cols="6">
          <v-card class="ml-auto" max-width="300" elevation="10">
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
          <v-card class="mr-auto" max-width="300" elevation="10">
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

    
    <div id="section5">
      <v-row justify="center" class="mt-4">
        <h1 class="h1 font-weight-bold mb-4 font text-center text-capitalize">
          My Experience at Chefs Academy
        </h1>
      </v-row>

      <v-row>
        <v-carousel
          cycle
          height="400"
          hide-delimiter-background
          show-arrows-on-hover
        >
          <v-carousel-item>
            <v-row justify="center" class="mt-8">
              <v-avatar color="primary" size="164">
                <img src="/grad3.jpg" />
              </v-avatar>
            </v-row>
            <v-row justify="center" class="mt-4">
              <div class="text-center mx-auto font mt-4">
                The professionalism at Chef's Academy is top notch and the
                quality <br />
                of services rendered are highly commendable. I'd recommend
                Chef's Academy not just for the value one gets but also for the
                amazing <br />
                learning experience that stays with you long after the end of
                the program
              </div>
            </v-row>
            <v-row justify="center" class="mt-4">
              <div class="text-center mx-auto font mt-4 overline">Amaka</div>
            </v-row>

            <v-row justify="center" class="mt-2">
              <div class="text-center mx-auto font mt-4 h4">GRADUATE</div>
            </v-row>
          </v-carousel-item>

          <v-carousel-item>
            <v-row justify="center" class="mt-8">
              <v-avatar color="primary" size="164">
                <img src="/grd1.jpg" />
              </v-avatar>
            </v-row>
            <v-row justify="center" class="mt-4">
              <div class="text-center mx-auto font mt-4">
                Training at Chef's Academy is the highlight of my professional
                career so far.<br />
                The wealth of knowledge taught and the practical application
                will launch anyone<br />
                who desires to go into the culinary world from a novice to a
                professional per excellence.
              </div>
            </v-row>
            <v-row justify="center" class="mt-4">
              <div class="text-center mx-auto font mt-4 overline">
                Anselm Ekere
              </div>
            </v-row>

            <v-row justify="center" class="mt-2">
              <div class="text-center mx-auto font mt-4 h4">GRADUATE</div>
            </v-row>
          </v-carousel-item>

          <v-carousel-item>
            <v-row justify="center" class="mt-8">
              <v-avatar color="primary" size="164">
                <img src="/grad2.jpg" />
              </v-avatar>
            </v-row>
            <v-row justify="center" class="mt-4">
              <div class="text-center mx-auto font mt-4">
                The professionalism at Chef's Academy is top notch and the
                quality of services rendered are highly commendable.<br />
                I'd recommend Chef's Academy not just for the value one gets but
                also for the amazing learning<br />
                experience that stays with you long after the end of the program
              </div>
            </v-row>
            <v-row justify="center" class="mt-4">
              <div class="text-center mx-auto font mt-4 overline">Tokunbo</div>
            </v-row>

            <v-row justify="center" class="mt-2">
              <div class="text-center mx-auto font mt-4 h4">GRADUATE</div>
            </v-row>
          </v-carousel-item>
        </v-carousel>
      </v-row>
    </div>

 

    <div id="section6">
      <v-row justify="center" class="mt-4">
        <h1 class="h1 font-weight-bold mb-4 font text-center text-capitalize">
          Some of Our Clients
        </h1>
      </v-row>

      <v-row class="mt-6 ml-0">
        <v-col cols="2">
          <v-img contain height="100" max-width="150" src="/hlt.svg"></v-img>
        </v-col>
        <v-col cols="2">
          <v-img height="100" contain max-width="150" src="nab.jpg"></v-img>
        </v-col>
        <v-col cols="2">
          <v-img contain height="100" max-width="150" src="jbc.png"></v-img>
        </v-col>
        <v-col cols="2">
          <v-img contain height="100" max-width="150" src="/fis.jpg"></v-img>
        </v-col>
        <v-col cols="2">
          <v-img contain height="100" max-width="150" src="cam.jpg"></v-img>
        </v-col>
        <v-col cols="2" class="">
          <v-img contain height="100" max-width="150" src="cer.jpg"></v-img>
        </v-col>
      </v-row>
    </div> -->
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

.v-sheet.v-card {
  border-radius: 5px;
}

.test {
  clip-path: circle(50% at 73% 43%);
}

.font {
  color: black;
}

.fnt-x {
  font-family: 'Poppins', sans-serif;
  font-size: 40px;
}

.fntc {
  font-family: 'Poppins', sans-serif;
  font-size: 20px;
}

.pusht {
  margin-top: 15%;
}

.t {
  background: #f2874a;
}

/* On screens that are 992px or less, set the background color to blue */
@media screen and (max-width: 992px) {
  .sec_space {
    margin-top: 15%;
  }
  .wordspace {
    margin-top: 15%;
  }
}

/* On screens that are 600px or less, set the background color to olive */
@media screen and (max-width: 600px) {
  .sec_space {
    margin-top: 15%;
  }
  .wordspace {
    margin-top: 30%;
  }
}

.wordspace {
  margin-top: 15%;
}

.sec_space {
  margin-top: 15%;
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
  background: #ffffff;
}

#section3 {
  width: 100vw;
  height: 50vh;
  overflow: hidden;
  background: #fffafa;
}

#section4 {
  width: 100vw;
  height: 100vh;
  overflow: hidden;
  background: #ffffff;
}

#section5 {
  width: 100vw;
  height: 100vh;
  overflow: hidden;
  background: #ffffff;
}

#section6 {
  width: 100vw;
  height: 50vh;
  overflow: hidden;
  background: #ffffff;
}

.newLand {
  clip-path: ellipse(62% 65% at 72% 34%);
  background: url('/newL.jpg');
  background-attachment: fixed;
  height: 100%;
}
</style>
