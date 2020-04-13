<template>
  <v-container class="back d-flex justify-space-evenly" fluid>
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
