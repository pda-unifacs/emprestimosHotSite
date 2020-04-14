<template>
  <v-col sm="6" elevation="6" cols="12">
    <v-card class="justify-center">
      <v-carousel
        class="mx-auto"
        cycle
        height="500"
        interval="5000"
        :show-arrows=false
      >
        <v-carousel-item
          v-for="(item,i) in items"
          :key="i"
        >
          <v-img
          :src="item.src"
          max-height="800"
          max-width="655"
          aspect-ratio="1.3"
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
      // { src: require('@/assets/img/1.png') },
      // { src: require('@/assets/img/2.png') },
      // { src: require('@/assets/img/3.png') }
    ]
  })
}
</script>

<style>

</style>
