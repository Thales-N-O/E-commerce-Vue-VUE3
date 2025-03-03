<template>
<input type="text" value="oi" v-model="texto" name="" id="">
<p>{{ texto }}</p>
</template>
<script setup>
import {ref} from "vue"
const texto=ref('vue e muito legal')
</script>
<style scoped></style>