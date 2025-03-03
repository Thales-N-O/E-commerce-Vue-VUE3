<template>
<h1>preços e itens</h1>
</template>
<script setup>
import { defineProps } from 'vue';

defineProps({
    item:String,
    preco:Number
})
</script>
<style scoped>p{color:black;}</style>