<template>
  <v-col sm="6" elevation="6" cols="12">
    <v-card class="justify-center">
      <v-carousel
        class="mx-auto"
        cycle
        height="850"
        interval="3000"
        :show-arrows=false
      >
        <v-carousel-item
          v-for="(item,i) in items"
          :key="i"
          :src="item.src"
        >
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
      { src: require('@/assets/img/app1.jpg') },
      { src: require('@/assets/img/app2.jpg') },
      { src: require('@/assets/img/app3.jpg') }
    ]
  })
}
</script>

<style>

</style>
