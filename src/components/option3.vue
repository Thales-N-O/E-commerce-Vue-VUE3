<template>
     
    <p> {{ item }} &  {{ preco }}</p>
    <button @click="adicionar"> Add to car</button>
    </template>
    <script setup>
    import { defineProps, defineEmits } from 'vue';
    
    const props=defineProps({
        item:String,
        preco:Number
    })
    const emit= defineEmits(["foiAdicionado"])
    function adicionar(){
        emit("foiAdicionado",props.preco)
    }
    </script>
    <style scoped>p{color:black;}</style>