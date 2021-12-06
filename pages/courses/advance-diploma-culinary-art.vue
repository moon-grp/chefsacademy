<template>
  <div>
    <v-row>
      <v-carousel :show-arrows="false" hide-delimiters height="50vh">
        <v-carousel-item src="/ad.JPG" aspect-ratio="1"></v-carousel-item>
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
        <div class="text-capitalize fon">About Advance Diploma in culinary art</div>

        <div class="mt-4 text-left fntcc">
          The diploma in culinary arts is a curriculum designed specifiaclly for
          students intrested in the culinary arts.<br />
          Students get high-quality academic, thoeretical, and foundational
          practical training in the areas of cooking,<br />
          pastry, and bakery, as well as service.
        </div>

        <div class="mt-4">
          <v-list-item two-line>
            <v-list-item-content>
              <v-list-item-title class="fntc"> Duration </v-list-item-title>
              <v-list-item-subtitle>12 weeks (5 days a week)</v-list-item-subtitle>
            </v-list-item-content>
          </v-list-item>

           <v-list-item two-line>
            <v-list-item-content>
              <v-list-item-title class="fntc"> Price </v-list-item-title>
              <v-list-item-subtitle>₦ 550,000 (5,000 registration fee)</v-list-item-subtitle>
            </v-list-item-content>
          </v-list-item>
        </div>

        <div class="mt-6">
          <v-btn  x-large color="#f2874a" dark  class="text-capitalize fntccc">
            apply
          </v-btn>
        </div>
        
      </v-container>
    </v-row>
  </div>
</template>

<script>
export default {
  layout: 'courses',
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
