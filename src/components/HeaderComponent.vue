<template>
<header>
    <h1>E-Commerce com Vue.js</h1><i class="fa-brands fa-vuejs"></i>
    
</header>
<nav>
    
<input id="codigador" v-model="MeuTexto" type="text">
<p>Procurar por: {{ MeuTexto }}</p>
</nav>
</template>
<script setup>
import{ref}from "vue"
const inputado=document.getElementById('codigador')
const MeuTexto=ref("")

</script>
<style scoped>
nav{
text-align: center important!;
  &>p{
    
    width: 50vw;
    word-wrap: break-word;    
  }}
</style>

