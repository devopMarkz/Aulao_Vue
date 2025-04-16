<script setup>
  import PrimeiroComponente from './components/PrimeiroComponente.vue';
  import ComDados from './components/ComDados.vue';
  import ComDadosReativos from './components/ComDadosReativosPrimitivos.vue';
  import ComDadosReativosNaoPrimitivos from './components/ComDadosReativosNaoPrimitivos.vue';
  import DataBinding from './components/DataBinding.vue';
</script>

<template>
  <header>vue</header>
  <PrimeiroComponente/>
  <ComDados nome="Caneta" codigo="321"/>
  <ComDadosReativos/>
  <ComDadosReativosNaoPrimitivos/>
  <DataBinding/>
</template>

<style scoped>
</style>
