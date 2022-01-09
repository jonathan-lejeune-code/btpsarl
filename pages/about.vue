<template>
  <v-container class="about section mt-10">
    <v-layout row wrap align-center>
      <v-flex xs12 sm6 px-3>
        <div class="about-thumb text-xs-center mb-4">
          <v-img
            src="https://www.expert-chantier.fr/assets/components/phpthumbof/cache/entreprise.f0e06343dbddff9666ef083d1ba8f9d4.jpg"
            aspect-ratio="1"
          ></v-img>
        </div>
      </v-flex>
      <v-flex xs-12 sm6 px-3>
        <div class="section-head">
          <h2 class="section-title">Presentation</h2>
          <div class="section-meta">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eaque
            voluptatibus iure, voluptates, saepe quos dolorum!
          </div>
        </div>

        <div class="section-body">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Similique
          aliquam, impedit. Blanditiis ab explicabo quidem saepe animi veniam,
          impedit ex sunt id quia vel totam? Lorem ipsum dolor sit amet
          consectetur, adipisicing elit. Expedita recusandae quasi eum vitae,
          dolores ab delectus sapiente quia, a vero molestiae assumenda impedit
          libero praesentium. Debitis, repellendus dolores. Reprehenderit,
          maiores.
        </div>
      </v-flex>
    </v-layout>

    <v-row>
      <v-col
        v-for="item in items"
        :key="item.id"
        class="mx-auto"
        cols="12"
        sm="4"
      >
        <v-card flat tile class="mx-auto mt-10">
          <v-img
            :src="item.src"
            aspect-ratio="1"
            class="grey lighten-2"
          ></v-img>
          <v-card-text class="text--primary text-center">
            <div class="title">{{ item.name }}</div>
            <p>{{ item.title }}</p>
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>
<script>
export default {
  name: 'AboutPage',
  components: {},

  data() {
    return {
      items: [
        {
          id: 1,
          src: 'https://static7.depositphotos.com/1192060/779/i/600/depositphotos_7794432-stock-photo-business-executive-stood-outdoors.jpg',
          name: 'Oliver Queen',
          title: 'PDG',
        },
        {
          id: 2,
          src: 'https://us.123rf.com/450wm/sevalv/sevalv1712/sevalv171200848/92324625-joli-sourire-joyeusement-f%C3%A9minin-aux-cheveux-blonds-habill%C3%A9-avec-d%C3%A9sinvolture-regardant-avec-satisfa.jpg?ver=6',
          name: 'Rachel Queen',
          title: 'Responsable RH ',
        },
        {
          id: 3,
          src: 'https://thumbs.dreamstime.com/b/portrait-de-jeune-homme-d-affaires-s%C3%A9rieux-avec-le-regard-intense-%C3%A0-l-appareil-photo-54810844.jpg',
          name: 'Peter Queen',
          title: 'Responsable Commercial ',
        },
      ],
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.about {
  position: relative;
  overflow: hidden;
}
</style>
