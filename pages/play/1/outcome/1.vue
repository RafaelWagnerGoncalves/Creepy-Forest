<template>
    <div>
        <BadEnding :title="['Corre o mais rápido possível','> A sua corrida não foi suficiente para superar a da manada. Você morreu atropelado.']"/>
    </div>
</template>

<script>
import BadEnding from '../../../../src/components/BadEnding.vue'

export default {

  components: {
    BadEnding,

  },
}
</script>

<style>

</style>