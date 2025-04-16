<script setup>
    import { ref } from 'vue';
    const valor = ref('');
</script>

<template>
    <div id="componente">
        <h1>Componente com Data Binding</h1>
        <input type="text" v-model="valor">
        <p>{{ valor }}</p>
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