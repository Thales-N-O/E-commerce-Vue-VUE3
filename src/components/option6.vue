<template>
<option5 @clicado="receber" item="Arroz"/>
<p>Modular secundário: {{ item }}</p>
<h1>Resultado da Emissão</h1>

</template>
<script setup>
import {ref} from "vue"
import option5 from './option5.vue';
const todosTexto=document.querySelectorAll('input')
todosTexto.forEach(e=>{
    console.log(e);
    
})
const receber=()=>{
    alert(texto.value)
    
}

</script>
<style scoped>

</style>