<template>
<h1>Teste de Emissão</h1>
<p>modular primário: {{ item }}</p>
<button @click="comprado"> Comprar</button>
<h1>btn2</h1>
<input type="text" name="" id="promotionCode">
<button @click="transmitir">Resgatar Pressente</button>
<p>Contagem: {{ estado.count }}</p>
<button @click="aumentar">+1</button>
</template>
<script setup>
import { defineProps,ref,defineEmits,reactive } from 'vue';
defineProps({
    item:String
})
const comprado=()=>{alert('efetue o pagamento')}
const estado = reactive({ count: 0 }) // Cria um objeto reativo
const aumentar = () => {
  estado.count++ // Atualiza o valor (Vue detecta e reflete no template)
}
const emit=defineEmits(['clicado'])
const transmitir=()=>{
    emit('clicado')
}
</script>
<style scoped>

</style>