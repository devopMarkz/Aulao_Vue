<script setup>

    const props = defineProps({
        item:String,
        preco:Number
    });

    // Os gritos que o componente filho pode dar para o pai ouvir
    const emit = defineEmits(['foiAdicionado']);

    function adicionar(){
         emit("foiAdicionado", props.preco);
    }

    
</script>

<template>

    <div>
        <h1>Componente que Emite Eventos</h1>
        <p> {{ item }} (R${{ preco.toFixed(2) }}) </p>
        <button @click="adicionar">Adicionar ao carrinho</button>
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