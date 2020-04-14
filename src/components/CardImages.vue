<template>
  <v-col sm="6" cols="12">
    <v-card raised>
      <v-carousel
        cycle
        height="526"
        :show-arrows=false
      >
        <v-carousel-item
          v-for="(item,i) in items"
          :key="i"
        >
          <v-img
          :src="item.src"
          aspect-ratio="1.15"
          contain
          >
          </v-img>
        </v-carousel-item>
      </v-carousel>
    </v-card>
  </v-col>
</template>

<script>
export default {
  name: 'CardImages',
  data: () => ({
    items: [
      { src: require('@/assets/img/app1.png') },
      { src: require('@/assets/img/app2.png') },
      { src: require('@/assets/img/app3.png') }
    ]
  })
}
</script>

<style>

</style>
