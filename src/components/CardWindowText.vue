<template>
  <v-col sm="6">
    <v-row dense>
      <v-col
        cols="12"
        v-for="(item,i) in items"
        :key="i"
      >
        <v-card raised dark>
          <div class="d-flex">
            <v-card-title
              id="bg-card-title"
              v-text="item.title"
            />
            <v-divider />
            <v-card-subtitle
              id="bg-card-subtitle"
              v-text="item.text"
            />
          </div>
        </v-card>
      </v-col>
    </v-row>
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
        title: 'Taxas?',
        text: 'Sem taxas adicionais ou qualquer outra tarifa nas suas transações'
      },
      {
        title: 'Simplicidade',
        text: 'Um design simples e intuitivo para você não ficar perdido'
      },
      {
        title: 'Quando você quiser',
        text: 'Mesmo sem internet desfrute das funções de "agendamento" para quando se conectar novamente'
      }
    ]
  })
}
</script>

<style>
  #bg-card-title {
    background: #4678D3;
  }

  #bg-card-subtitle {
    background: whitesmoke;
    color: black;
  }
</style>
