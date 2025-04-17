<script setup>
import EmiteEvento from './EmiteEvento.vue';
import { ref } from 'vue';

const total = ref(0);

function atualizarTotal(preco){
    total.value += preco;
    total.value.toFixed(2);
}
</script>
 
<template>
    <div class="pai-eventos">
        <h1>Componente que Escuta Evento</h1>
        <p>Total: R${{ total }}</p>
        <div class="eventos">
            <EmiteEvento item="Item1" :preco="1.99" @foiAdicionado="atualizarTotal"/>
            <EmiteEvento item="Item2" :preco="5.00" @foiAdicionado="atualizarTotal"/>
            <EmiteEvento item="Item3" :preco="10.99" @foiAdicionado="atualizarTotal"/>
        </div>
    </div>
</template>

<style scoped>
    .pai-eventos{
        text-align: center;
        border: 2px solid rgb(10, 69, 4);
        background-color: #050d04;
    }

    .eventos{
        display: flex;
        text-align: center;
        border-radius: 15px;
        margin: 30px;
        padding: 10px;
    }
</style>