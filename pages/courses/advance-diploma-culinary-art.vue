<template>
  <div>
    <v-row>
     
       <v-carousel :show-arrows="false" hide-delimiters height="50vh">
        <v-carousel-item src="https://res.cloudinary.com/sparaclet-inc/image/upload/v1645211747/chefsacademy/photo5800683805667867023_n1krg5.jpg" aspect-ratio="16/9"></v-carousel-item>
      </v-carousel>

     <!--   <v-app-bar
        absolute
        color="#6A76AB"
        dark
        shrink-on-scroll
        prominent
        src="/newL.JPG"
        contain
        height="180"
      >
        <v-row justify="center" align="center" class="mt-16">
          <div>Diploma in culinary art</div>
        </v-row>
      </v-app-bar> -->
    </v-row>
    <v-row class="mt-4">
      <v-container class="mb-6">
        <div class="text-capitalize fon">
          Advance Diploma in culinary art and food entrepreneurial management
        </div>

        <div class="mt-4 text-left fntcc">
          Master the art of pastries, baking cookery and more in our advanced
          diploma<br />
          in culinary arts and entrepreneurial management. You will explore
          diffrent african menus,<br />
          experiment with ethnic and contemporary cuisine as well as develop
          your skills in the <br />
          culinary arts while learning valuable managment skills that will take
          your carrer to the next level.
        </div>

        <div class="mt-4">
          <v-list-item two-line>
            <v-list-item-content>
              <v-list-item-title class="fntc"> Duration </v-list-item-title>
              <v-list-item-subtitle
                >14 weeks (4 days a week)</v-list-item-subtitle
              >
            </v-list-item-content>
          </v-list-item>

          <v-list-item two-line>
            <v-list-item-content>
              <v-list-item-title class="fntc"> Tution fee </v-list-item-title>
              <v-list-item-subtitle
                >₦ 550,000 (5,000 registration fee)</v-list-item-subtitle
              >
            </v-list-item-content>
          </v-list-item>
        </div>

        <div class="mt-6">
          <v-btn
            x-large
            color="#f2874a"
            dark
            class="text-capitalize fntccc"
            @click="dialog = true"
          >
            apply
          </v-btn>
        </div>
      </v-container>
    </v-row>
    <v-dialog v-model="dialog" persistent max-width="600px">
      <v-card>
        <v-card-title>
          <span class="text-h5">Application form</span>
        </v-card-title>
        <v-card-text>
          <v-container>
            <v-row>
              <v-col cols="12" sm="6" md="6">
                <v-text-field
                  label="First name"
                  v-model="firstname"
                  outlined
                ></v-text-field>
              </v-col>

              <v-col cols="12" sm="6" md="6">
                <v-text-field
                  label="Last name"
                  v-model="lastname"
                  outlined
                ></v-text-field>
              </v-col>
              <v-col cols="12">
                <v-text-field
                  label="Email"
                  v-model="email"
                  outlined
                ></v-text-field>
              </v-col>
              <v-col cols="12">
                <v-text-field
                  label="Phone number"
                  type="number"
                  outlined
                  v-model="phonenumber"
                ></v-text-field>
              </v-col>
              <v-col cols="12">
                <v-text-field
                  label="Address"
                  v-model="address"
                  outlined
                ></v-text-field>
              </v-col>
            </v-row>
          </v-container>
          <small>*indicates required field</small>
        </v-card-text>
        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn color="blue darken-1" text @click="dialog = false">
            Close
          </v-btn>
          <v-btn color="blue darken-1" text @click="send_application">
            Save
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
    <v-snackbar
      shaped
      outlined
      type="success"
      v-model="alert"
      top
      :timeout="7000"
    >
      we would contact you shortly..
    </v-snackbar>
  </div>
</template>

<script>
import { SfBanner } from '@storefront-ui/vue'
import axios from 'axios'
export default {
  layout: 'courses',
   components: {
    SfBanner,
  },
  data() {
    return {
      alert: false,
      firstname: null,
      lastname: null,
      email: null,
      phonenumber: null,
      dialog: false,
      address: null,
      course: 'Advanced diploma in culinary art',
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
  methods: {
    send_application() {
      var _name = this.firstname + ' ' + this.lastname
      axios
        .post('https://chefsacademybot.herokuapp.com/notify', {
          name: _name,
          email: this.email,
          phonenumber: this.phonenumber,
          address: this.address,
          course: this.course,
        })
        .then((res) => {
          this.dialog = false
          this.alert = true
        })
    },
  },
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@600&display=swap');

.sf-banner {
  height: 10vh;
  font-family: 'Urbanist', sans-serif;
  --banner-height:
}




.v-sheet.v-card {
  border-radius: 5px;
}

.test {
  clip-path: circle(50% at 73% 43%);
}

.fon {
  font-family: 'Poppins', sans-serif;
  font-size: 30px;
  color: #f2874a;
}

.fnt {
  font-family: 'Poppins', sans-serif;
  font-size: 20px;
}

.fntcc {
  font-family: 'Poppins', sans-serif;
  font-size: 15px;
}

.fntccc {
  font-family: 'Poppins', sans-serif;
}

.section1 {
  height: 5vh;
}

.v-btn:not(.v-btn--round).v-size--x-large {
  height: 52px;
  width: 200px;
  padding: 0 23.1111111111px;
}
</style>
