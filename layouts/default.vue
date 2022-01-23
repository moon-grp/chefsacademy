<template>
  <v-app dark app>
    <v-main class="bg">
      <v-app-bar elevate-on-scroll color="transparent" absolute>
        <v-toolbar-title class="ml-6">
          <nuxt-link to="/">
            <v-avatar size="55" tile>
              <v-img class="mx-2" src="https://res.cloudinary.com/sparaclet-inc/image/upload/v1642946453/chefsacademy/logo_qkxw9s.jpg"></v-img>
            </v-avatar>
          </nuxt-link>
        </v-toolbar-title>
        <v-spacer></v-spacer>

        <nuxt-link to="/">
          <v-btn
            color=""
            text
            class="text-capitalize mx-2 hidden-sm-and-down fnt"
            >Home</v-btn
          >
        </nuxt-link>
        <nuxt-link to="/">
          <v-btn
            color=""
            text
            class="text-capitalize mx-2 hidden-sm-and-down fnt"
            >About us</v-btn
          >
        </nuxt-link>

        <nuxt-link to="#courses">
          <v-btn
            color=""
            text
            class="text-capitalize mx-2 hidden-sm-and-down fnt"
            >Courses</v-btn
          >
        </nuxt-link>
      </v-app-bar>

      <Nuxt class="mb-15" />
      
    <!--  <v-footer padless>
        <v-card flat tile  class="text-center" color="">
          <v-card-text>
            <span class="fntxxx"> +234 809 218 9734 | +234 815 563 3650 </span
            ><br />
            <v-btn text color="">
              <v-icon left> mdi-map-marker </v-icon>
              33, parakou cresent, off aminu Kano cresent, wuse 2, abuja
            </v-btn>
            <br />

            <v-btn text color="">
              <v-icon left> mdi-email </v-icon>
              chefsacademy@gmail.com
            </v-btn>
            <br />
            <v-btn text color="">
              <v-icon left> mdi-twitter </v-icon>
              chefsacademyng
            </v-btn>

            <v-btn text color="">
              <v-icon left> mdi-facebook </v-icon>
              chefsacademyng
            </v-btn>

            <v-btn text color="">
              <v-icon left> mdi-instagram </v-icon>
              chefsacademyng
            </v-btn>
          </v-card-text>
        </v-card>
      </v-footer> -->
    </v-main>

    <!--   <v-footer :absolute="!fixed" app>
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer> -->

    <v-footer padless color="#FFFFFF">
      <v-row justify="center" align="center" class="hidden-md-and-down">
        <v-card flat tile  class="text-center" color="#FFFFFF">
          <v-card-text>
            <span class=""> +234 809 218 9734 | +234 815 563 3650 </span
            ><br />
            <v-btn text color="">
              <v-icon left> mdi-map-marker </v-icon>
              33, parakou cresent, off aminu Kano cresent, wuse 2, abuja
            </v-btn>
            <br />

            <v-btn text color="">
              <v-icon left> mdi-email </v-icon>
              chefsacademy@gmail.com
            </v-btn>
            <br />
            <v-btn text color="">
              <v-icon left> mdi-twitter </v-icon>
              chefsacademyng
            </v-btn>

            <v-btn text color="">
              <v-icon left> mdi-facebook </v-icon>
              chefsacademyng
            </v-btn>

            <v-btn text color="">
              <v-icon left> mdi-instagram </v-icon>
              chefsacademyng
            </v-btn>
          </v-card-text>
        </v-card>
      </v-row>
      </v-footer>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/',
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire',
        },
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js',
    }
  },
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@600&display=swap');

html {
  font-family: 'Poppins', sans-serif;
}

.containe {
  background-image: url('~assets/land1.png');
}

.bg {
  background: #ffffff;
}

.fnt {
  font-family: 'Poppins', sans-serif;
  font-size: 25px;
}

.fntxxx {
  font-family: 'Poppins', sans-serif;
  font-size: 15px;
}

a {
  text-decoration: none;
}
</style>
