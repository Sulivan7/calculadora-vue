<script setup>
import { reactive } from 'vue';
import Header from './components/Cabecalho.vue';
import Form from './components/formulario.vue';

const estado = reactive({
  valor1: "",
  valor2: "",
  filtro: 'adicao',
});

function calcular() {
  switch (estado.filtro) {
    case 'adicao':
      return estado.valor1 + estado.valor2;
    case 'subtracao':
      return estado.valor1 - estado.valor2;
    case 'multiplicacao':
      return estado.valor1 * estado.valor2;
    case 'divisao':
      return estado.valor2 !== 0 ? estado.valor1 / estado.valor2 : 'Operação inválida: divisor não pode ser zero.';
    default:
      return 'Operação inválida';
  }
}
</script>

<template>
  <div class="container">
    <Header />
    <Form :trocar-filtro="(event) => (estado.filtro = event.target.value)"
      :valor1="(event) => (estado.valor1 = Number(event.target.value))"
      :valor2="(event) => (estado.valor2 = Number(event.target.value))" />
      
      <div class="footer">
        <h2 class="mt-4 fs-2">Resultado {{ calcular() }}</h2>
      </div>
    </div>
</template>

<style scoped>
.container {
    max-width: 600px;
    margin: auto;
    padding: 20px;
}

.footer {
    text-align: center;
    margin-top: 20px;
    background-color: #f8f9fa;
    padding: 10px;
    border-radius: 5px;
  }
</style>
