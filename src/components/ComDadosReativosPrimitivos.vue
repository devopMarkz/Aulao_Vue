<script setup>
    import { ref } from 'vue';
    const nome = ref("André");
    const idade = ref(22);

    function fazerAniversario() {
        idade.value += 1;
    }

    function mudarNome(){
        nome.value = "Ana Maria Braga";
    }
</script>

<template>
    <div>
        <h1>Componente com dados reativos</h1>
        <p>Nome: {{ nome }} - Idade: {{ idade }}</p>
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