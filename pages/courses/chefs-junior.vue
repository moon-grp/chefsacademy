<template>
  <div>
    <v-row>
      <v-carousel :show-arrows="false" hide-delimiters height="50vh">
        <v-carousel-item src="https://res.cloudinary.com/sparaclet-inc/image/upload/v1645342668/chefsacademy/photo5805348436504066363_wlhy4x.jpg" aspect-ratio="1"></v-carousel-item>
      </v-carousel>

      <!--  <v-app-bar
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
         Chefs's academy junior
        </div>

        <div class="mt-4 text-left fntcc">
         Our kids are not left out, we have planned short courses for kids from age seven years.<br/>
         We teach etiquette, basic pastry, cooking skills, kitchen and fire safety.
        </div>

     <!--   <div class="mt-4">
          <v-list-item two-line>
            <v-list-item-content>
              <v-list-item-title class="fntc"> Duration </v-list-item-title>
              <v-list-item-subtitle
                >5 weeks(3 days a week)</v-list-item-subtitle
              >
            </v-list-item-content>
          </v-list-item>

          <v-list-item two-line>
            <v-list-item-content>
              <v-list-item-title class="fntc"> Price </v-list-item-title>
              <v-list-item-subtitle
                >₦ 355,000 (5,000 registration fee)</v-list-item-subtitle
              >
            </v-list-item-content>
          </v-list-item>
        </div> -->

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
import axios from 'axios'
export default {
  layout: 'courses',
  data() {
    return {
      alert: false,
      firstname: null,
      lastname: null,
      email: null,
      phonenumber: null,
      dialog: false,
      address: null,
      course: 'professional diploma',
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
