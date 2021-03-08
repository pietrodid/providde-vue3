<template>
<h1>App contador: {{contador}}</h1>
<Contador />
<contador-accion />
</template>

<script>
import {provide, ref} from 'vue'
import Contador from './components/Contador.vue'
import ContadorAccion from './components/ContadorAccion.vue'
export default {
  components: {Contador, ContadorAccion},
  name: 'App',
  
  setup() {
    const contador = ref (0)

    provide('contador', contador)

    return {contador}
  }
}
</script>

