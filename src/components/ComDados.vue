<script setup>
    const defineProps = defineProps(['nome', 'codigo']);
</script>

<template>
    <div>
        <h1>Componente com dados</h1>
        <p>Nome: {{ nome }} - {{ codigo }}</p>
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