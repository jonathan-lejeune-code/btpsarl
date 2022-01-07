<template>
  <v-container>
    <h1>bienvenue sur le site BTP SARl</h1>
    <v-row>
      <v-col cols="12" class="mt-15">
        <v-carousel
          class="hidden-xs-only"
          cycle
          height="600"
          hide-delimiter-background
          :show-arrows="false"
        >
          <v-carousel-item
            v-for="(item, i) in items"
            :key="i"
            :src="item.src"
          ></v-carousel-item>
        </v-carousel>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'IndexPage',

  data: () => ({
    items: [
      {
        src: `https://i.f1g.fr/media/eidos/805x453_crop/2020/03/19/XVMb02b559c-69cd-11ea-a29b-4b821834e44f.jpg`,
      },
      {
        src: `https://www.metiers-btp.fr/wp-content/uploads/2019/04/SECTEUR_BTP_440726068_1920px.jpg`,
      },
      {
        src: `https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQryxsuamKa4itJ3ATQ0P0ndeT2R4P4hbszXxBHa1sHEBvTADY-iXdIysPMLe93O9uHE6c&usqp=CAU`,
      },
      {
        src: `https://img.batiweb.com/repo-images/article/36178/sondage.jpg`,
      },
    ],
  }),
}
</script>
