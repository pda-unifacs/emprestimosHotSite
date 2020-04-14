<template>
  <v-container class="d-flex">
      <v-row class="stretch">
        <CardImages/>
        <CardWindowText/>
      </v-row>
  </v-container>
</template>

<script>
import CardImages from '@/components/CardImages.vue'
import CardWindowText from '@/components/CardWindowText.vue'

export default {
  name: 'Home',
  components: {
    CardImages,
    CardWindowText
  }
}
</script>

<style>

</style>
