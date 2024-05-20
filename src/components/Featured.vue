<template>
  <v-row>
    <v-col cols="3" sm="3" v-for="(feature, i) in featured" :key="i">
      <v-card class="mx-auto my-12 pb-4" max-width="374">
        <v-img height="250" class="mx-4" :src="feature.img"></v-img>
        <v-card-item class="mt-n4">
          <v-card-title class="text-center">{{ featured.title }}</v-card-title>
        </v-card-item>
        <v-card-text>
          <div class="text-center">
            {{ feature.bio }}
          </div>
          <v-row align="center" class="mx-0 mt-2">
            <v-rating
              :model-value="4.5"
              color="ambor"
              density="compact"
              half-increment
              readonly
              size="small"
            ></v-rating>
            <v-spacer></v-spacer>
            <div class="text-grey ms-4">{{ feature.price }}</div>
          </v-row>
        </v-card-text>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
export default {
  data() {
    return {
      featured: [
        {
          img: "image/1.jpg",
          title: "Product Name",
          price: "1222฿",
          bio: "Product Bio",
        },
        {
          img: "image/2.jpg",
          title: "Product Name",
          price: "1222฿",
          bio: "Product Bio",
        },
        {
          img: "image/3.jpg",
          title: "Product Name",
          price: "1222฿",
          bio: "Product Bio",
        },
        {
          img: "image/4.jpg",
          title: "Product Name",
          price: "1222฿",
          bio: "Product Bio",
        },
      ],
    };
  },
};
</script>

<style>
</style>