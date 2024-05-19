<template>
  <v-app>
    <v-main>
      <NavBar />
      <v-container>
        <v-row>
          <v-col cols="12">
            <v-carousel>
              <v-carousel-item
                v-for="(item, i) in items"
                :key="i"
                :src="item.src"
                cover
              >
                <v-row class="fill-height">
                  <v-col cols="12" sm="6">
                    <div class="d-flex fill-height justify-center align-center">
                      <h2 class="text-white top">{{ item.title }}</h2>
                    </div>
                  </v-col>
                </v-row>
              </v-carousel-item>
            </v-carousel>
          </v-col>
        </v-row>
      </v-container>
    </v-main>
  </v-app>
</template>

<script setup>
import NavBar from "../components/NavBar.vue";
</script>

<script>
export default {
  data() {
    return {
      items: [
        {
          src: "1.jpg",
          title: "Zulfa Studio",
          text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua",
        },
        {
          src: "2.jpg",
          title: "Zulfa Studio",
          text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua",
        },
        {
          src: "3.jpg",
          title: "Zulfa Studio",
          text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua",
        },
        {
          src: "4.jpg",
          title: "Zulfa Studio",
          text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua",
        },
        {
          src: "5.jpg",
          title: "Zulfa Studio",
          text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua",
        },
        {
          src: "6.jpg",
          title: "Zulfa Studio",
          text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua",
        },
        {
          src: "7.jpg",
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
  margin-top: -40px;
  margin-left: 80px;
}
.top-day {
  margin-top: 120px;
}
</style>
