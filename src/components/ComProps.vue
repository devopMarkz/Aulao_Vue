<script setup>
    import {defineProps} from 'vue';

    const props = defineProps(['item', 'preco']);

    
</script>

<template>

    <div>
        <h1>Componente com Props</h1>
        <p> {{ item }} (R${{ preco }}) </p>
    </div>

</template>

<style scoped>
    
</style>