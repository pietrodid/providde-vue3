<template>
    <h1>contador:{{contador}} </h1>
</template>

<script>
import { inject } from 'vue'

export default {
  setup(){
      const contador = inject('contador')

      return {contador}
  }
}
</script>
