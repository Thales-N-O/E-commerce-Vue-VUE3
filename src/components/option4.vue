<template>
   
        <span>total: R${{ total }}</span>
        <div>
    <option3 item="item1" :preco="20.99" @foiAdicionado="atualizarTotal"/>
    <option3 item="item2" :preco="49.99"@foiAdicionado="atualizarTotal"/>
    </div>
</template>

<script setup>
 import { ref } from 'vue';
import option3 from './option3.vue';
 const total =ref(0)
 function atualizarTotal(p){
    const valor=total.value + p
    total.value = +valor.toFixed(2)
 }
</script>
<style scoped>
div{display: flex;align-items: center; gap: 2vw;}
</style>