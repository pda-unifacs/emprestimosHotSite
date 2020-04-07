<template>
  <v-col sm="6" elevation="6" cols="12">
    <v-card>
        <!-- TODO: Adicionar 'show-arrows' e tentar resolver bug de ambos 'prev/next'
                   estarem no mesmo lado
        -->
      <v-carousel
        class="mx-auto"
        cycle
        :show-arrows=false
        interval="3000"
      >
        <!-- TODO: Adicionar imagens quando terminar o prototipo das telas -->
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
      { src: '@/assets/img/img1.jpg' },
      { src: '@/assets/img/2.jpg' },
      { src: '@/assets/img/3.jpg' },
      { src: '@/assets/img/4.jpg' }
    ]
  })
}
</script>

<style>

</style>
