<template>
<button @click="contador ++">Aumentar</button>
<button @click="contador --">Disminuir</button>
</template>

<script>
import {inject} from 'vue'
export default {
    setup() {
        const contador = inject('contador')

        return {contador}
    }
}
</script>

