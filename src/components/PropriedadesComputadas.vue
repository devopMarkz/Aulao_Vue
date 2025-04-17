<script setup>
import { ref, computed } from 'vue';

const nome = ref('');
const sobrenome = ref('');

const nomeCompleto = computed(() => {
    return nome.value + " " + sobrenome.value;
});

</script>

<template>

    <div id="componente">
        <h1>Componente com Propriedades Computadas</h1>
        <input type="text" v-model="nome">
        <input type="text" v-model="sobrenome">
        <p>Nome Completo: {{ nomeCompleto }}</p>
    </div>

</template>

<style scoped>
    div{
        text-align: center;
        border: 2px solid rgb(10, 69, 4);
        background-color: #050d04;
        border-radius: 15px;
        margin: 30px;
        padding: 10px;
    }
</style>