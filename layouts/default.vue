<template>
  <v-app dark app>
    <v-main>
      <v-app-bar   elevate-on-scroll absolute color="transparent" >
        <v-toolbar-title class="ml-6">
          <nuxt-link to="/">
            <v-avatar size="50">
              <v-img class="mx-2" src="/logo.jpg"></v-img>
            </v-avatar>
          </nuxt-link>
        </v-toolbar-title>
        <v-spacer></v-spacer>

        <nuxt-link to="/affiliate">
          <v-btn dark text class="text-capitalize mx-2 hidden-sm-and-down fnt"
            >Home</v-btn
          >
        </nuxt-link>
        <nuxt-link to="/affiliate">
          <v-btn dark text class="text-capitalize mx-2 hidden-sm-and-down fnt"
            >About us</v-btn
          >
        </nuxt-link>

        <nuxt-link to="/affiliate">
          <v-btn dark text class="text-capitalize mx-2 hidden-sm-and-down fnt"
            >Courses</v-btn
          >
        </nuxt-link>

        <nuxt-link to="/affiliate">
          <v-btn text dark class="text-capitalize mx-2 hidden-sm-and-down fnt"
            >consultancy services</v-btn
          >
        </nuxt-link>

        <nuxt-link to="/affiliate">
          <v-btn dark text class="text-capitalize mx-2 hidden-sm-and-down fnt"
            >gallery</v-btn
          >
        </nuxt-link>
        <v-spacer></v-spacer>
      </v-app-bar>

      <Nuxt class="mt-0" />
    </v-main>

 <!--   <v-footer :absolute="!fixed" app>
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer> -->
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

.containe {
  background-image: url('~assets/land1.png');
}

body {
  background: #ffffff;
}

.fnt {
  font-family: 'Poppins', sans-serif;
  font-size: 20px;
  color: #000000;
}

a {
  text-decoration: none;
}
</style>
