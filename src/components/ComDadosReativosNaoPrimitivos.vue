<script setup>
    import { reactive } from 'vue';

    const pessoa = reactive({
        nome: "Marcos",
        idade: 22
    });

    function fazerAniversario() {
        pessoa.idade += 1;
    }

    function mudarNome(){
        pessoa.nome = "Ana Maria Braga";
    }
</script>

<template>
    <div>
        <h1>Componente com dados reativos</h1>
        <p>Nome: {{ pessoa.nome }} - Idade: {{ pessoa.idade }}</p>
        <button @click="fazerAniversario">Fazer aniversário</button>
        <button @click="mudarNome">Mudar Nome</button>
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