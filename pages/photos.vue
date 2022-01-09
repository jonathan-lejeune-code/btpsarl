<template>
  <v-app>
    <h2 class="section-title" bloc>Photos</h2>
    <v-row>
      <v-col v-for="n in 25" :key="n" class="d-flex child-flex" cols="2">
        <v-img
          :src="`https://www.marc-chazelle.fr/images/entreprise/chantier-7.jpg`"
          aspect-ratio="1"
          class="grey lighten-2"
          @click.stop="dialog = true"
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
      <v-dialog v-model="dialog" max-width="720" isDark="">
        <v-card>
          <v-img
            :src="`https://www.marc-chazelle.fr/images/entreprise/chantier-7.jpg`"
            max-width="720"
            height="auto"
          ></v-img>
          <v-card-actions>
            <v-spacer></v-spacer>

            <v-btn @click="dialog = false" color="red darken-1" text>
              Close
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-dialog>
    </v-row>
  </v-app>
</template>

<script>
export default {
  name: 'PhotosPage',
  data() {
    return {
      dialog: false,
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
