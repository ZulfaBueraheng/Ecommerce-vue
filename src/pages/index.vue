<template>
  <v-app>
    <v-main>
      <NavBar />
      <v-container>
        <v-row>
          <v-col cols="12" sm="12">
            <v-carousel>
              <v-carousel-item
                v-for="(item, i) in items"
                :key="i"
                :src="item.src"
                cover
              >
                <v-row class="fill-height">
                  <v-col cols="12" sm="6">
                    <div
                      class="d-flex flex-column justify-center align-center text-center"
                    >
                      <h2 class="text-white top">{{ item.title }}</h2>
                      <p class="text-white text">{{ item.text }}</p>
                      <v-btn class="btn-buy">Buy Now</v-btn>
                    </div>
                  </v-col>
                </v-row>
              </v-carousel-item>
            </v-carousel>
          </v-col>
          <v-toolbar color="transparent">
            <v-toolbar-title>Popular Product</v-toolbar-title>
            <v-spacer></v-spacer>
            <v-btn icon="mdi mdi-chevron-left"></v-btn>
            <v-btn icon="mdi mdi-chevron-right"></v-btn>
          </v-toolbar>
          <v-col cols="12" sm="12" class="mt-n10">
            <Popular />
          </v-col>
          <v-toolbar color="transparent" class="mt-n10">
            <v-toolbar-title>Featured Product</v-toolbar-title>
            <v-spacer></v-spacer>
            <v-btn icon="mdi mdi-chevron-left"></v-btn>
            <v-btn icon="mdi mdi-chevron-right"></v-btn>
          </v-toolbar>
          <v-col cols="12" sm="12" class="mt-n10">
            <Featured />
          </v-col>
        </v-row>
      </v-container>
    </v-main>
  </v-app>
</template>

<script setup>
import NavBar from "../components/NavBar.vue";
import Popular from "../components/Popular.vue";
import Featured from "../components/Featured.vue";
</script>

<script>
export default {
  data() {
    return {
Client
      items: [
        {
          src: "image/1.jpg",
          title: "Zulfa Studio",
          text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua",
        },
        {
          src: "image/2.jpg",
          title: "Zulfa Studio",
          text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua",
        },
        {
          src: "image/3.jpg",
          title: "Zulfa Studio",
          text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua",
        },
        {
          src: "image/4.jpg",
          title: "Zulfa Studio",
          text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua",
        },
        {
          src: "image/5.jpg",
          title: "Zulfa Studio",
          text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua",
        },
        {
          src: "image/6.jpg",
          title: "Zulfa Studio",
          text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua",
        },
        {
          src: "image/7.jpg",
          title: "Zulfa Studio",
          text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua",
        },
      ],
    };
  },
};
</script>

<style scoped>
.top {
  margin-top: 100px;
}
.text {
  margin-top: 20px;
  margin-left: 80px;
}
.btn-buy {
  margin-top: 20px;
}
.top-day {
  margin-top: 120px;
}
</style>
