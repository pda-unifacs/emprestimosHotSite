<template>
  <v-col sm="6">
    <v-card>
      <v-row dense>
        <v-col
          cols="12"
          sm="12"
          elevation="6"
          v-for="(item,i) in items"
          :key="i"
        >
          <v-card dark>
            <div class="d-flex flex-no-wrap justify-space-between">
              <div>
                <v-card-title class="justify-center" v-text="item.title"/>
                <v-card-subtitle v-text="item.text"/>
              </div>
            </div>
          </v-card>
        </v-col>
      </v-row>
    </v-card>
  </v-col>
</template>

<script>
export default {
  name: 'CardWindowText',
  data: () => ({
    items: [
      {
        title: 'Serviço Premium',
        text: 'Serviços de alta qualidade com transparencia em todas as transações'
      },
      {
        title: 'Taxa?',
        text: 'Sem taxas adicionais ou qualquer outra tarifa nas suas transações'
      }
    ]
  })
}
</script>

<style>

</style>
