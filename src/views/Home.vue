<template>
  <v-container class="back d-flex justify-center" fluid>
    <v-row>
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
