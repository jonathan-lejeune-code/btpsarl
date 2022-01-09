<template>
  <v-app>
    <h2 class="section-title" bloc>Photos</h2>
    <v-row>
      <v-col v-for="n in 50" :key="n" class="d-flex child-flex" cols="2">
        <v-img
          :src="`https://picsum.photos/500/300?image=${n * 5 + 10}`"
          :lazy-src="`https://picsum.photos/10/6?image=${n * 5 + 10}`"
          aspect-ratio="1"
          class="grey lighten-2"
        >
          <template v-slot:placeholder>
            <v-row class="fill-height ma-0" align="center" justify="center">
              <v-progress-circular
                indeterminate
                color="grey lighten-5"
              ></v-progress-circular>
            </v-row>
          </template>
        </v-img>
      </v-col>
    </v-row>
  </v-app>
</template>

<script>
export default {
  name: 'PhotosPage',
  data() {
    return {
      items: [
        // {
        //   id: 1,
        //   src: '../assets/images/GP/img1.webp',
        // },
      ],
    }
  },
}
</script>

<style lang="scss" scoped>
h2 {
  background-color: orange;
  border-radius: 10px;
  font-size: 50px;
  margin: 10px auto;
}
</style>
